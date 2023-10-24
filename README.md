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
[Creating actions](https://docs.github.com/en/actions/creating-actions)  
[Metadata syntax for GitHub Actions - runs.pre](https://docs.github.com/en/actions/creating-actions/metadata-syntax-for-github-actions#runspre)  
[Creating a JavaScript action](https://docs.github.com/en/actions/creating-actions/creating-a-javascript-action)  
[GitHub Actions Toolkit](https://github.com/actions/toolkit)  
[Assigning permissions to jobs](https://docs.github.com/en/actions/using-jobs/assigning-permissions-to-jobs)  

## Other repositories from the same course
[second-action-react-demo](https://github.com/brunosantanati/second-action-react-demo)  
[github-actions-time-to-practice](https://github.com/brunosantanati/github-actions-time-to-practice)  
[events-deep-dive](https://github.com/brunosantanati/events-deep-dive)  
[github-actions-data](https://github.com/brunosantanati/github-actions-data)  
[github-actions-env](https://github.com/brunosantanati/github-actions-env)  
[github-actions-execution-flow](https://github.com/brunosantanati/github-actions-execution-flow)  
[github-actions-containers](https://github.com/brunosantanati/github-actions-containers)  
[github-actions-custom-actions](https://github.com/brunosantanati/github-actions-custom-actions)  
[github-actions-security](https://github.com/brunosantanati/github-actions-security)  

## Some commands used throughout the course
```
npm outdated
npm update
```

## Default Environment Variables

It was shown in the course how to set and use your own environment variables.

GitHub Actions also provides a couple of default environment variables that are set automatically: https://docs.github.com/en/actions/learn-github-actions/environment-variables#default-environment-variables

These environment variable can, for example, give you quick access to the repository to which the workflow belongs, the name of the event that triggered the workflow and many other things.  

## Storing Actions In Repositories & Sharing Actions With Others

In this module, we created custom Actions that were stored in the same repository as our Workflow(s).

Alternatively, we could've stored the custom Actions in separate repositories (which therefore then only include the Action definition + code).

This is actually quite straightforward:

1. Create a new, local project folder which contains your action.yml file + all the code belonging to the action (Important: Don't put your action.yml file or code in a .github/actions folder or anything like that - just keep it directly on the root level of your created project!)

1. Add a local Git repository to your created project (via git init)

1. Create your commit(s) via git add and git commit

1. Create a GitHub repository and connect it to your local Git repository (via git remote add)

1. Add a tag via git tag -a -m "My action release" v1

1. Push your local code to the remote GitHub repository (via git push --follow tags)

1. Use your custom Action in any other Workflow (in any other project and repository) by referencing the repository which contains your action (e.g., my-account/my-action@v1)

If your custom Action is stored in a public repository, it can also be published to the GitHub Actions Marketplace as described here: https://docs.github.com/en/actions/creating-actions/publishing-actions-in-github-marketplace#publishing-an-action  

## More On GitHub Actions Security

In addition to the concepts covered in this module, you should absolutely also explore the security guides by GitHub itself:

- General overview & important concepts: https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions

- More on Secrets: https://docs.github.com/en/actions/security-guides/encrypted-secrets

- Using GITHUB_TOKEN: https://docs.github.com/en/actions/security-guides/automatic-token-authentication

- Advanced - Preventing Fork Pull Requests Attacks: https://securitylab.github.com/research/github-actions-preventing-pwn-requests/

- Security Hardening with OpenID Connect: https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect
