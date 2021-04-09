# Git workflow

## Setting up

Fork the Code Collabo repo you want to work on - e.g. [node-mongo-cli](https://github.com/code-collabo/node-mongo-cli).

Open up your terminal on your computer and do the following:

* Clone that forked version onto your computer with:

  `git clone git@github.com:your-github-username/node-mongo-cli.git`

  If you prefer or are using https:

  `git clone https://github.com/your-github-username/node-mongo-cli.git`

* Set original repo as upstream:

  `git remote add upstream git@github.com:code-collabo/node-mongo-cli.git`

Check that your forked repo's url is set as the origin & original repo's url is set as the upstream with: `git remote -v`

## Updating your fork

Setting original repo as the upstream means you'll be able to update your fork, with the latest changes made to the original repo using the `git pull` command.

Before you start or as you work on the code, update your fork so that you'll be working with latest changes from the original repo.

To pull changes for the develop branch for example, checkout to develop: `git checkout develop`

Then use the command: `git pull`

In summary, just checkout to the branch you want to pull changes into `git checkout branch-name` and use the `git pull` command.

## Gitflow and branches

The only time you have business with the main branch is if you choose to pull changes while in the main branch as explained in _**updating your fork**_.

📌 _**You are not to make changes to main branch, as it contains the production-ready version of the code**_.

A branch with name `develop` has been created for development purpose.

📌 _**Also, you are not to make changes to the develop branch**_. Instead, **create a** `feature branch` **from the develop branch** and make your changes there.

## Creating a feature branch

* Checkout to develop to ensure the feature branch you will create is a copy of the develop branch: `git checkout develop`
* Create a feature branch while inside develop branch: `git checkout -b feature-branch-name-here`

| 📌 Note |
| :--- |


Always make sure you checkout to develop branch before creating a new feature branch.

## Naming a feature branch

To help admin/reviewers know what you are working on, give your feature branch a descriptive name containing: `issueNumber-action-description`.

* **IssueNumber:** Check the issue to get issue number. 
* **Action:** Words like `fix`,  `setup`,  `feature` etc. 
* **Description:** What you are setting up, fixing etc.

  So, feature branch name could look like `7-setup-jasmine-test`,  `19-update-readme`, `1001-fix-db-error` etc.

## Submitting your changes

After you've made the needed changes in the feature branch you created, follow these steps:

### Add & commit your changes

`git add .`

`git commit -m "Add your commit message here"`

### Push changes

Push your changes to the remote for the first time: `git push -u origin your-branch-name`

Push every other time: `git push`

### Pull request

Next create & send a `pull request` so that your code can be reviewed. Also add description & testing checklist to your pull request. See examples of previously made pull requests for how to go about this:

* [Pull request 7](https://github.com/code-collabo/node-mongo-cli/pull/11#issue-584788302) 
* [Pull request 21](https://github.com/code-collabo/node-mongo-cli/pull/21#issue-589792008)

| [Docs home](https://github.com/code-collabo/docs) | [Contributor guide](https://github.com/code-collabo/docs/tree/main/contributor-guide) |
| :--- | :--- |


