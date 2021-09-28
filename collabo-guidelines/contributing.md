---
description: General and project-specific guidelines
---

# Contribution guidelines

Thank you for your interest in Code Collabo. You are welcome to contribute to any of Code Collabo's projects regardless of your level of experience. Do make sure to read up the code of conduct, general guidelines for Code Collabo projects and the guidelines specific to the project you wish to work on.

{% hint style="info" %}
Contribution guideline is different depending on the project you are working on.
{% endhint %}

## General guidelines for Code Collabo projects

First check to see if a project's repo has a **develop branch**. If the project's repo has a develop branch, then create your **feature branch** from the develop develop. If there is no develop branch, then create your feature branch from the **main branch**. Do not make changes directly in the main branch or the develop branch. See [git workflow](https://code-collabo.gitbook.io/docs/contributor-guide/git-workflow) for explanation of these terms, how to make changes to a project's code base and submit pull request.

{% hint style="info" %}
Do not make changes directly in the develop branch or the main branch.
{% endhint %}

It is also possible that two or more persons can be working on the same issue or same parts of the code without knowing it. First check whether the issue you want to work is in the issues tab on Github. If you find the issue there, check to see f it has been assigned to someone. If not, request to be assigned. If the issue is not there on Github, raise the issue and get assigned to it. This way, who is working on what is visible to everyone and we will be able to avoid conflicts. Additionally, the issues created will be added to the project board to track a project's progress and will help writing project release notes.

{% hint style="info" %}
Make what you are working on visible to everyone to avoid conflicts, to help track a project's progress and what will be added to the project's release notes.
{% endhint %}

## Project-specific contribution guidelines

Find guidelines specific to a particular project in the project's overview page:



## Git workflow

This tutorial will use [node-mongo-cli](https://github.com/code-collabo/node-mongo-cli) as example. Use the repo name of the repo you want to work on instead, if it is not the node-mongo-cli. The ssh .git urls are used here, so ensure that you have [set up your connection to Github with ssh](%20https://docs.github.com/en/authentication/connecting-to-github-with-ssh). Or you can just replace the ssh urls with the http url if you prefer or are using http.

### Setting up

**Step 1 -** Fork the Code Collabo repo you want to work on. Open up your terminal on your computer.

**Step 2 -** Clone that forked version onto your computer:

```text
git clone git@github.com:your-github-username/node-mongo-cli.git
```

**Step 3 -** Set original repo as upstream: 

```text
git remote add upstream git@github.com:code-collabo/node-mongo-cli.git
```

You can check that your forked repo's .git url is set as the origin, and the original repo's .git url is set as the upstream with:

```text
git remote -v
```

## Updating your fork

Setting original repo as the upstream means you'll be able to update your fork, with the latest changes made to the original repo using the **git pull** command. Before you start or as you work on the code, update your fork so that you'll be working with latest changes from the original repo.

To pull changes for the develop branch, checkout to develop: 

```text
git checkout develop
```

Then use any of the git pull commands below depending on which works for you:

```text
git pull
```

```text
git pull upstream develop
```

The above pulls the latest changes unto your local computer, but does not yet reflect in the remote origin i.e. the forked repo in your Github account. Update the remote origin with this command:

```text
git push origin develop
```

Replace the word develop with main in the commands above in case you want to checkout to main branch and pull in changes for the main branch.

## Gitflow and branches

The main branch contains the production-ready version of the code. Only create a feature branch from the main branch if you do not find a branch named "develop".

{% hint style="info" %}
You are not to make changes to **main branch**, as it contains the production-ready version of the code.
{% endhint %}

The develop branch is created for development purpose.

{% hint style="info" %}
Also, you are not to make changes to the **develop branch**. Instead, **create a feature branch** **from the develop branch** and make your changes there.
{% endhint %}

## Creating a feature branch

Checkout to develop to ensure the feature branch you will create is a copy of the develop branch:

```text
git checkout develop
```

Create a feature branch while inside develop branch:

```text
git checkout -b feature-branch-name-here
```

{% hint style="info" %}
Always make sure you checkout to develop branch before creating a new feature branch.
{% endhint %}

## Submitting your changes

After you've made the needed changes in the feature branch you created, add, commit, push and submit a pull request.

Add changes:

```text
git add .
```

Commit changes:

```text
git commit -m "Add your commit message here"
```

Push changes from your feature branch to the remote: 

```text
git push origin your-branch-name
```

You can then go ahead to [create and send a pull request from your fork](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork) so that your code can be reviewed.

## Further study

Although the sections above are what you will be needing to contribute, see [this YouTube resource](https://youtu.be/jFL228SfOmU) to help understand the git workflow term better.

