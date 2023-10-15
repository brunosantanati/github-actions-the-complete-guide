# [GitHub Actions - The Complete Guide](https://www.udemy.com/course/github-actions-the-complete-guide/)

## Links
[Original Repo](https://github.com/academind/github-actions-course-resources)  
[About GitHub-hosted runners](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners/about-github-hosted-runners)  
[Events that trigger workflows](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows)  
[GitHub Action Checkout](https://github.com/actions/checkout)  
[Contexts](https://docs.github.com/en/actions/learn-github-actions/contexts)  
[Skipping workflow runs](https://docs.github.com/en/actions/managing-workflow-runs/skipping-workflow-runs)  
[Using inputs and secrets in a reusable workflow](https://docs.github.com/en/actions/using-workflows/reusing-workflows#using-inputs-and-secrets-in-a-reusable-workflow)  
[About service containers](https://docs.github.com/en/actions/using-containerized-services/about-service-containers)  

## Other repositories from the same course
[second-action-react-demo](https://github.com/brunosantanati/second-action-react-demo)  
[github-actions-time-to-practice](https://github.com/brunosantanati/github-actions-time-to-practice)  
[events-deep-dive](https://github.com/brunosantanati/events-deep-dive)  
[github-actions-data](https://github.com/brunosantanati/github-actions-data)  
[github-actions-env](https://github.com/brunosantanati/github-actions-env)  
[github-actions-execution-flow](https://github.com/brunosantanati/github-actions-execution-flow)  
[github-actions-containers](https://github.com/brunosantanati/github-actions-containers)  

## Some commands used throughout the course
```
npm outdated
npm update
```

## Default Environment Variables

It was shown in the course how to set and use your own environment variables.

GitHub Actions also provides a couple of default environment variables that are set automatically: https://docs.github.com/en/actions/learn-github-actions/environment-variables#default-environment-variables

These environment variable can, for example, give you quick access to the repository to which the workflow belongs, the name of the event that triggered the workflow and many other things.
