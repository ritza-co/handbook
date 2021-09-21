# Understanding the differences between deployment guides and tutorials

On Code Capsules we have both Deployment Guides and Tutorials.

## Deployment guies
Deployment Guides are for everyone. They are reference guides. They do not aim to teach the reader anything, only to get the reader up-and-running on Code Capsules as fast as possible. The reader should be able to go "I want to build an application using $X (e.g. MERN, Python, whatever) and I want a good starting point that is production-ready". The should be able to pick the guide that matches their stack, and knowing nothing about Code Capsules be able to follow the step-by-step instructions to have an example application deployed.

They can then modify this code, and still have a production application hosted in the same stack by simply modifying the code and running

```
git add .
git commit -m "my updates"
git push
```

Deployment guides should be completely focused on the infrastructure and configuration. They should not show any code samples, but just link to an example repl which has a minimal example app. These apps should not be "interesting" (e.g. a job board, chat bot etc), but should just be the absolute minimum that a reader needs. This is often simply a "hello world" app, or in the case of e.g. the MERN application, an interactive version to show the minimum of frontend + backend + database + inserting into and reading from the database.

## Tutorials

Tutorials are for beginners. They should *teach* concepts, and have extensive code samples. They should demo *interesting* applications - not just hello worlds or To Do lists that have been done thousands of times before. Here the reader is learning to code, and doesn't want to think about hosting or deployment. Ideally, the tutorial should link out to a relevant deployment guide (e.g. the MERN Job Board links to MERN deployment guide), and say 'do this first'. With all the config out of the way, the tutorial can focus only on the code used to build the app, and then show how to use git to add the new changes, test locally if appropriate, and push to CC to deploy to production. 

## Target audiences

People of all levels will use the deployment guides - beginners because they want to host their portfolio or similar and don't know anything about hosting or DevOps. Experienced engineers because they haven't used Code Capsules before and don't want to read the documentation, so they will scan through and copy any configuration or see where to click specific UI buttons.

Examples:

* Alice is a senior engineer. She has used many other hosting solutions, but now wants to use Code Capsules because it has low latency to her target audience in Africa. She has her application already built and just wants to deploy it. It is written in Django and backed by a MySQL Database, so she runs through first the Django deployment guide and then the MySQL deployment guide to set up both of those capsules. She substitutes the GitHub URLs for her pre-built application instead of using the example applications - because she is experienced, this is easy for her and she doesn't need to be told how to do this explicitly.
* Bob is a junior developer. He has never hosted anything before and he has no code to start from. He wants to build something for his portfolio, but isn't sure what. He follows the MERN deployment guide step-by-step, exactly, including using the same URLs to the sample application. He gets a hello world application running with a database backend. He isn't sure what to do next. He scans through the tutorials and decides to build a job board. It links back to the guide he just followed. He continues to follow everything exactly step-by-step, not needing to make any changes specific to his own app and soon he has a job board deployed. He understands how everything works because he read the text as well as following along step by step to build out the code.


