# Project Bub

A personal website project.

## Overview

This document contains the process that will be used to develop code for the application as well as the requirements needed to be completed for this project to be complete.

## Development Cycle

To make the development of this project easy, a simple cycle will be used that will use `git` and **GitHub** to complete.

### Step 0 - Create Issues

Create the _Issues_ in **GitHub** so that work can be complete. This will be done by me so I can help with the flow of the project. This will also allow you to code more and think about the work less.

### Step 1 - Pick an Issue

Pick an _Issue_ from **GitHub** to work on and create a new local branch.

```bash
git branch -b <branch_name>
```

The `<branch_name>` should include your initials, the issue number, and a shorthand description as follows:

```bash
<initials>/<issue_number>-<shorthand_desc>

Example:
tr/1-create-spec
```

### Step 2 - Do the work

Complete the work the is described in the description of the _Issue_ that you are currently working on. Make sure that you do not do more work than the ticket describes. If you are unsure if something is within the "scope" of the ticket, just ask.

### Step 3 - Push the code

Once the work for the ticket is complete locally on your machine, `push` it to **GitHub**

```bash
git push
```

If it is the first time you are `push`-ing your branch to **GitHub** you may need to also set the `upstream`. The upstream is the name of the remote repository that you are trying to `push` to. This will usually be `origin`.

```bash
git push --set-upstream <remote_name> <branch_name>

Example:
git push --set-upstream origin tr/1-create-spec
```

**Make sure that you are not `push`-ing to the `master` branch and only to the branch create for the issue.**

### Step 4 - Start Code review

Once you have pushed your code to **GitHub**, create a _Pull Request_ in **GitHub** to request that I review your work. Once you have done that, send me the link to the PR (_Pull Request_).

When you create the _Pull Request_, in the description make sure to include

### Step 5 - Resolve Code Review comments

If there are any changes that need to be made for the PR, I will comment about them with direction on how to fix them in the PR. Feel free to ask questions on why and/or what needs to be done.

You will need to update your local repository and `push` the changes for the fixes to **GitHub** similar to Step 3, however you will need to make sure that you are on the same branch that the PR is for.

Once all of the comments in the PR are resolved, merging the branch to master is ready to happen.

### Step 6 - Merge to Master

Click the _Merge_ button in the PR (in **GitHub**) to merge the branch to master. This will add all of your changes to the master branch and complete work on the current ticket.

## Specifications

The following information outlines the specifications of the work. If there are any questions, please ask before work starts.

### General Specs

* The website must be responsive. This means that the site must adjust how it is viewed on both a web browser and a mobile browser. [Bootstrap](https://getbootstrap.com/) may help with doing this

* The website will have "gutters" to the left and right to ensure that the text and assets fill the screen in a visually appealing way.

* All assets (images, graphics, etc.) must be Creative Commons Zero properties.  What this means is that they are public domain and free to use and modify without attribution.

* Feel free to use any other library that you would like to enhance the design.
#### Additional Info

| Requirement                  | Helpful Info                                                                             |
| ---------------------------- | ---------------------------------------------------------------------------------------- |
| Responsive Design            | [HTML Responsive Web Design](https://www.w3schools.com/html/html_responsive.asp)         |
| Responsive Design            | [Bootstrap](https://getbootstrap.com/)                                                   |
| Creative Commons Zero Assets | [CC0 1.0 - Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/) |
| Creative Commons Zero Assets | [Unsplash Image Library](https://unsplash.com/)|
| Useful Site | [Font Awesome](http://fontawesome.io/) |
| Useful Site | [Hero Patterns](http://www.heropatterns.com/) |

### Color Palette
The following is the general color palette that I would like used for the site.  

[Color Palette](./swatches.html)

### Site Design

This site will have only a handful of sections that are outlined below.  Each section may have multiple __Issues__ raised to get the work complete.  Additionally, the content of these sections will be provided in *JSON* format and added into the section via **JavaScript**. I will help you with this step and it will be one of the last things we do. 

#### Header
The Header should be 300px - 400px tall and show either an interesting photograph, image, or pattern.  I will provide a log to place here at a later date.

Overlayed to the top right of the header should be a LinkedIn, Twitter, and GitHub icons that can be clicked to navigate to the respective app.

#### Page Navigation
There should be a navigation bar directly underneath the header.  Since this is a single page site, clicking these links should simply scroll you to that location on the page.  The following links should be available:

* Home => Sends to top of page

* About Me => Sends to the About Me section

* Contact Me => Sends to Contact Me section

#### About Me
This section will provide a brief description about me and what I do.  There should be space for a picture of me to the left with the text to the right.  My name should be an `h1` above the image and text.

Expect 2-3 paragraphs of text when mocking the text.

#### Section Break
This section is going to be three columns that each have an image and some text the describe my primary skills.  This section will not have a section header.  I will provide the images at a later time.

#### Contact Me

This section will have information on how to contact me and should include the following:

* Email Address
* LinkedIn
* Twitter

Feel free to make this section interesting with subtle usage of graphics as you see fit.

#### Footer

This should include a "created by" sentance and copyright info that lets people know that you made the page and when it was created.  

### Examples of Design

The following are some links to pages that you a design similar to what I want:

[Scientist Site](https://www.wix.com/website-template/view/html/1596?originUrl=https%3A%2F%2Fwww.wix.com%2Fwebsite%2Ftemplates%2Fhtml%2Fportfolio-cv%2Fpersonal%2F1&bookName=create-master-new&galleryDocIndex=1&category=portfolio-cv&metaSiteId=)
## Appendix

## Using GitHub

### Clone

This allows you to `clone` a **GitHub** repository

```bash
git clone git@github.com:CoppyLobbies/project_bub.git
```

### Status

This displays the current status of your local repository

```bash
git status

Output:

On branch tr/1-create-spec
Your branch is up-to-date with 'origin/tr/1-create-spec'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   spec/README.md
```

### Pull

This updates your local repository to the most recent commit on your current branch

```bash
git pull
```

### Checkout

Allows you to switch between local branches or create a new branch

```bash
git checkout <branch_name>

Example:
git checkout tr/1-create-spec
```

If you add `-b` it will create the branch locally

```bash
git checkout -b <new_branch_name>

Example:
git checkout -b tr/2-shorthand-desc
```

### Push

Sends the current branch to the remote repository (**GitHub** as `origin`).

If you have already pushed the branch to the remote repository, you will just need the following command

```bash
git push
```

However, if you are pushing for the first time you will need to set the `upstream` which is the name of the remote repository and branch

```bash
git push --set-upstream <remote_name> <branch_name>

Example:
git push --set-upstream origin tr/1-create-spec
```

### Add

This "stages" a file or selection of files so that they can be committed. A file must be "staged" before it is committed (saved) to the repository.

```bash
git add <file_path>

Example:
git add file.html # adds a single file

git add .         # adds all files in current directory and subfolders

git add path/     # adds all files in a directory
```

### Commit

Creates a commit or "save" with everything that was "staged" via the `git add` command and adds it to the local repository in the current branch.

```bash
git commit
```

This will open up a text editor in your command line that requires you to add a commit message. Since this command line editors are hard to use at first, I would suggest adding `-m` when committing and including the message in the command

```bash
git commit -m "enter a message here with qoutes"
```
