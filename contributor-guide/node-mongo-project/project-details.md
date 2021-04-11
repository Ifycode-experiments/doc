# Project details

## Introduction

Hi, thank you for your interest to collabo\(rate\) and contribute to @code-collabo's **node-mongo project**. Straight to the point =&gt; I want every next project involving nodejs and mongoDB to be dead easy for me. A project which will also be useful to others be it a contributor or user.

I will talk about the project in detail under the following headings:

* About project.
* Who can contribute, prerequisites & tools.
* Project breakdown.
* Project timeline \(1st release\).
* Related repos & resources. 
* First task.

## About project

Like the name _**node-mongo**_ suggests, we will be working on package\(s\) built with nodejs and will involve mongoDB. This will include a [cli](https://github.com/code-collabo/node-mongo-cli) and [starter-kit](https://github.com/code-collabo/node-mongo-starter-kit). The starter-kit will have 3 templates - `es6`, `cjs` and `ts-es6` i.e. templates for es6+ syntax, commonJS syntax and typescript. The project is inspired by angular framework \(and the likes\).

### Our cli is to work in this manner \(1st release\):

* Use commands to install/create a new mongoDB project, adding our [starter-kit's](https://github.com/code-collabo/node-mongo-starter-kit) folders and files with their respective content into the project.
* The cli will be interactive. For example, asking if the user wants to use typescript in the project the user is creating. This way it will know what packages, file extensions or content to install. 

We will split the above mentioned tasks into much smaller tasks and open issues for them as the project progresses.

The project is likely to expand with more features e.g. authentication, updated releases from time to time and will therefore be needing maintenance.

### Problems it will help solve \(1st release\):

* Make the work of the mongoDB developer easier: Developer no longer needs to create project \(folders, files, packages\) from scratch. The CLI will help do this with ease.
* Javascript development environment already set up \(automation, linting, handling concurrent tasks etc\). All they need to do is run `npm start` to get the project running - as long as mongoDB is running locally on their computer or connected to mongoDB atlas \(cloud\).
* Help migrate from commonJS pattern/syntax \(although the cli will add commonjs in its options for those that want to use it\). 
* Apart from these, the project generated from the CLI will be made in a way that even frontend developers with little or no knowledge of MongoDB/database can use it \(there'll be option for this too\). 

  For example, they'll be able to get simple crud operations up and running. More like they'll just be "customizing" the Schema structure and response to their own taste.

  The documentation will be simple enough to help them with it.

It also hopes to provide real world, problem solving _**open source experience**_ for those new to open source contribution, _**internship experience**_ that contributors involved can comfortably add to resume or CV and _**remote work experience**_ for any one interested. I believe being a part of such project can help contribute to us being accepted, by other organizations we approach for those of us looking for job opportunities. The experience is also linked to an organisation \(Code Collabo\) and involves collabo\(ration\) which makes it even better.

## Who can contribute, prerequisites & tools.

* Anyone interested will be welcomed to contribute to the project. 
* Contributors must have knowledge of git, javascript & nodejs. MongoDB knowledge will be needed for those that want to contribute to the parts involving mongoDB.

### Important! 📌

Completing the [first task](https://github.com/code-collabo/docs/blob/main/contributor-guide/node-mongo-project/first-task.md) is compulsory for issues that have `cli-only` or `starter-kit-only` labels on them. It is to prepare those interested in contributing to the major part of the project for learning how to make a nodejs cli, and understanding the modifications we will be making to the node-mongo-cli project.

### Generally, you will need these to contribute:

* Nodejs 
* Git 
* MongoDB
* Postman

## Project breakdown

You can be involved in any or all of the following:

* Updating the [node-mongo-starter-kit](https://github.com/code-collabo/node-mongo-starter-kit).
* Making the typescript version of [node-mongo-starter-kit](https://github.com/code-collabo/node-mongo-starter-kit) in another repo so that we can add it to the CLI select options that will pop up in the terminal while user is creating a new project. Also useful if cloned or zipped from github.
* Making the commonJS version for same reason stated above.
* Scaffolding: Help with file and folder \(names and\) structure of the nodejs and mongoDB code to meet production standards.
* Make the cli \(commands, interaction, programming it to do what is in the about project description\).
* Testing.
* Documentation.
* Publish to npm 🎉

## Project timeline

Node-mongo-cli project \(officially\) started on 16th of March, 2020. All previous activities before this date were attempts to set up the repo. The estimated time to complete the work to be done in the **first release** is 2 and half months \(16th March, 2021 - 31st May, 2021\) - considering that helper resources have been added to help contributors.

## Related repos & resources

_**Related repos**_:

* [node-mongo-cli](https://github.com/code-collabo/node-mongo-cli).
* [node-mongo-starter-kit](https://github.com/code-collabo/node-mongo-starter-kit).
* [node-mongo-starter-cjs](https://github.com/code-collabo/node-mongo-starter-cjs).
* [node-mongo-docs](https://github.com/code-collabo/docs).

_**Resources**_:

[Find project resources here](https://github.com/code-collabo/docs/blob/main/contributor-guide/node-mongo-project/resources.md).

Pardon me for writing such a long text. It's so you can get a comprehensive and clear picture of what the project will achieve. Thanks for patiently reading through.

Please proceed to [first task](https://github.com/code-collabo/docs/blob/main/contributor-guide/node-mongo-project/first-task.md) 👈🏽

Obiagba Mary, Code Collabo Community.

