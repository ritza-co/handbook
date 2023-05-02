```
#!/opt/homebrew/bin/python3
import mimetypes 
import os
import sys
import uuid

import boto3
from dotenv import load_dotenv

load_dotenv()

def main():
    filepath = sys.argv[1]
    filename = os.path.basename(filepath)
    
    session = boto3.session.Session()
    client = boto3.resource('s3',
        region_name="ams3",
        endpoint_url="https://ritzastatic-com.ams3.digitaloceanspaces.com",
        aws_access_key_id=os.getenv("DO_ACCESS_KEY_ID"),
        aws_secret_access_key=os.getenv("DO_SECRET_ACCESS_KEY"),
    )
    content_type = ""
    try:
        content_type = mimetypes.MimeTypes().guess_type(filepath)[0]
    except:
        print("couldn't get content type")
    ui = uuid.uuid4().hex
    bucket = f"images"
    keyname = f"{ui}/{filename}"
    client.Bucket(bucket).upload_file(filepath, keyname, ExtraArgs={'ACL':'public-read', 'ContentType':content_type})
    url = f"https://i.ritzastatic.com/{bucket}/{keyname}"
    print(url)
    cmd = f'echo {url} | tr -d "\n" | pbcopy'
    os.system(cmd)

if __name__ == "__main__":
    main()

```
