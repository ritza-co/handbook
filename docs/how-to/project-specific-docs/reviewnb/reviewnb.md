# ReviewNB

* ReviewNB's main blog repository is in GitLab. We have a fork in GitHub.
* We have a shared GitLab account that you can use to authenticate with their (private) repo.
* Drafting, editing and QA should happen in our GitHub
* This branch can then be pushed to GitLab for their feedback

## Production process and Git

Generally, our flow is brief -> draft -> QA -> editing -> publish. **Upstream** is ReviewNB's repository on GitLab. **Origin** is our fork of this on GitHub.

* Production creates a brief and iterates on it with ReviewNB in a Google Doc
* QA creates a branch off upstream main and pushes it to origin, and shares the name in the channel.
* The author fetches this branch and pushes up commits of the article content directly to the branch
* QA pushes commits to the branch
* Editing pushes commits to the branch
* QA pushes the branch to an upstream branch
* Production opens an MR to upstream and emails ReviewNB to let them know that the post is ready for review

<img width="1073" alt="image" src="https://user-images.githubusercontent.com/2641205/210336750-61c10e97-559f-4b62-baec-26d02f9065eb.png">

## Setting up GitHub and GitLab remotes locally

You should have the code locally on your machine connected to both GitHub and GitLab remotes. You can use the GitHub UI to merge pull requests (e.g. editing, QA) into the draft branch. Once it's ready, you can push the draft branch to GitLab using the CLI and open a PR from the gitlab:draft-branch -> gitlab:main using the GitLab UI.

Clone our repository as `origin` and set theirs as `upstream`.

```
git clone git@github.com:ritza-co/reviewnb-blog.git
cd reviewnb-blog.git
git remote add upstream https://gitlab.com/amit1rrr/reviewnb-blog.git
```

Now you can push commits from our repository to branches in their repository. 

```
# fetch all updates from GitHub
git fetch origin

# switch to the draft branch
git checkout <draft-branch>

# push it to GitLab
git push upstream <draft-branch>
```

After running the last command, you'll get a link that lets you create a PR in the GitLab UI into main, which can be reviewed by ReviewNB before being merged.


```
reviewnb$ git push sandbox test
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 10 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (6/6), 456 bytes | 456.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: To create a merge request for test, visit:
remote:   https://gitlab.com/ritza-co/sandbox-2/-/merge_requests/new?merge_request%5Bsource_branch%5D=test
remote:
To https://gitlab.com/ritza-co/sandbox-2.git
 * [new branch]      test -> test
```

