---
title: Git, GitHub, & Markdown Resources
layout: page
---

## Contents
{:.no_toc}

- list
{:toc}

## Git, Github, and Markdown

<img src="https://avatars.githubusercontent.com/u/583231?v=4" alt="GitHub OctoCat" width="150px">

- [Git](https://git-scm.com/) - open-source software for version control
- [GitHub](https://github.com/) - a popular code repository for sharing and collaborating
- [Markdown](https://www.markdownguide.org/) - a lightweight, human-readable markup language

### Git

- What it does
  - Version control!
  - Git keeps track of file changes and enables you to label them and preserve multiple version histories of a project
- Why use it?
  - Avoid file conflicts! Other collaboration/syncing tools are not designed for code
  - It helps you test code, troubleshoot, or 'undo' changes
  - Be intentional: package your changes logically, document and explain your work

### [GitHub](https://www.github.com) 

<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="100px" alt="octocat logo">

- What does it do?
   - It hosts code and enables users to manage collaboration on projects (using Git for version control).
- Why use it?
  - Widely used to develop and share open-source tools and datasets
  - Free web hosting with static site builder ([GitHub Pages](https://pages.github.com/))
  - Makes collaboration visible and transparent

### [Markdown](https://www.markdownguide.org/) 

- It's a markup language: it encodes information in plain-text to be machine readable. Markdown uses the file extension `.md`
- Why use it?
  - Sustainable, open-source word-processing
  - Easier to read and write than HTML & other markup languages
  - Can be converted into any kind of document - including presentations like this one!
  - Used on many platforms (GitHub, Notion, Obsidian, Roam...)


### Vocabulary

**Repo or repository** (n.) 
: A discrete project on GitHub that contains a set of files, a change history, and a set of contributors. (E.g. [this one](https://github.com/digbmc/dssf-syll))

**Fork** (v.)
: To copy a repo's files and version history to a new one with its own settings (preserves connection with original repo but doesn't interfere). 

**Clone** (v.)
: To download a local copy of a repo on GitHub with a tracked connection to the remote repo.

**Local** (adj.)
: On your computer.

**Remote** (adj.)
: On someone else's computer (aka 'the cloud').

**Branch** (n.)
: A version of a repository with its own history. Branches can be created for a unique set of changes and later *merged* with the main branch to avoid file conflicts.

**Commit**
: (v.) To package and label a discrete set of changes to a repository.
: (n.) A set of changes that has been committed.


# 2. Writing in Markdown


```markdown
# First level heading 

## Second-level heading

Paragraph with **bold** text and *italicized* text. 

[This is linked text](www.myurl.com)

![This is an image with alt text](imageurl.jpg)
```

See this [cheat sheet](https://www.markdownguide.org/cheat-sheet/) for more markdown syntax.

# Your Turn

1. In Visual Studio Code, create a new file (**File > New File**) named `myfile.md`
2. Open the file and write some content using markdown syntax: include headers, images, and links
3. Save your file
4. On the left sidebar, right-click on the filename and select **Open Preview** to see what your site looks like in rendered markdown

# 3. Using GitHub

We'll take a tour of a **repository** for an open-source word cloud generator

[amueller/word_cloud](https://github.com/amueller/word_cloud)

![word cloud of US constitution](https://raw.githubusercontent.com/amueller/word_cloud/main/examples/constitution.png)

# How to create a repository

> - Create an empty repository on GitHub or import one from your computer
> - Copy an existing repository (by **forking** or using a **template**)
> - Add recommended files: a README.md for documentation, a license and a .gitignore

# Your turn

## Create a repo from a template

> - Navigate to the repo for this workshop: [github.com/digbmc/git-hub-ws](https://github.com/digbmc/git-hub-ws)
> - Click on **Use this template** and then **Create a new repository**
> - Give your repository a name and a description
> - Select 'copy only main branch'
> - Your new repository has the same files and change history, but not a tracked connection to the original

# Editing and uploading content

<section>
- Use the pencil icon to edit the README.md file
- Add some text and save your work using the **Commit changes** button
- Change the **commit message** so that it describes your changes 
- Select 'commit directly to the main branch' and click **Commit changes**
</section>

<section>
- Now let's upload the markdown file you created earlier.
- Back in your browser, select **Add file > Upload files**. 
- Drag and drop `myfile.md` into your repository
- Add a message when you **commit** your changes
</section>

# 4. Branching & Collaboration with Git

# Branching [workflow](https://docs.github.com/en/get-started/quickstart/github-flow)

<section class="left">
Branches make collaboration easier by avoiding file conflicts
![github branching diagram](https://docs.github.com/assets/cb-42360/images/help/repository/branching.png)
</section>

<section>
1. Commit changes to a new **branch** that diverges from the main tree
2. Open a pull request to propose your changes
3. A team member reviews the pull request and discusses any conflicts
4. Merge pull request: incorporate your changes into the main branch
</section>

<section>

## Your turn

> 1. Make another edit to your README.md file and **Commit** it
> 3. **Commit** your change and add a commit message
> 5. This time select 'create a new branch & open a pull request'
> 6. Review & **merge** the pull request
> 7. Look at your repository's commit history
</section>

# 5. Working locally

Git enables you to have a **local** version of your repository (on your computer) that is connected to the **remote** (on 'the cloud') version. 

By **pulling** commits from remote to local and **pushing** commits from local to remote, you can control the version history of both.

# Installing Git


## GitHub Desktop

Install a GUI client (an application with a graphical user interface) such as [GitHub desktop](https://desktop.github.com/)


## Command line

[Install Git here](https://git-scm.com/downloads) to use it from the command line and/or use Git/GitHub features for [VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#:~:text=Visual%20Studio%20Code%20has%20integrated,on%20the%20VS%20Code%20Marketplace.) or another text editor
</section>

# Configuration

## GitHub Desktop

- Open GitHub Desktop
- From the top menu, under GitHub Desktop: Preferences > Accounts > GitHub.com > Sign in
- Sign in using your GitHub account credentials


## Visual Studio Code 

- In VS code, navigate to the **Source Control** tab
- You will be prompted to sign in to GitHub and authorize VS code with your github account
- [see also these instructions](https://code.visualstudio.com/docs/sourcecontrol/overview)

## Command line
Open a terminal window and type:

`git config --global user.name "Firstname Lastname"`

When you push, you will have to authenticate to github with a [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)

# Clone the repository

- Create a folder on your computer for workshops (if you don't already have one)


## Visual Studio Code 

- In the **Source Control** tab, you will see an option to **Clone a repository**
- Select the new repository you have created

## GitHub Desktop

- Navigate to your new repository on github. From the 'Code' dropdown menu:
- Select 'Open with GitHub Desktop' and put it in the workshop folder
- Open the folder in VS Code (add folder to workspace)


## Command line

- Navigate to your new repository on github. From the 'Code' dropdown menu:
- Copy the url ending with .git. In your terminal, navigate to the workshop folder and type
`git clone [git url]`
- Open the folder in VS Code (add folder to workspace)


# 6. Git Versioning process

# Git workflow


## Add or Stage changes

`git add newfile.md`

After you create a new file or save changes, staging tells Git to track the file.

## commit 

`git commit -m "message describing my changes"`

Package your staged changes and label them for others' awareness


## pull

`git pull`  

Update your local repo with any changes that have been committed to the remote repo


## push

`git push origin main`

Send your changes to the remote repository and publish them on GitHub

## Other commands 

> - `git status` - see if you have staged changes
> - `git branch branchname` - create a new branch
> - `git checkout branchname` - switch to another branch


# Your turn

- Make some changes and save the files.
- Stage your changes: 
  - In VS Code, use the plus icon to stage a change
  - `git add --all`
- Commit your changes, with a message
  - Enter a message into the 'message' field and select 'Commit'
  - `git commit -m "message"`
- After a few commits, push to the remote repo: 
  - "Publish Branch"
  - `git push origin main`


![xkcd comic on Git](https://imgs.xkcd.com/comics/git.png)

Remember, it's ok to mess up! Source: [xkcd](https://xkcd.com/1597/)



# Resources

<h4 class="left">Git</h4>

- Git command line [cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [GitHub Desktop](https://desktop.github.com/), a GUI client for Git
- Git features in [VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#:~:text=Visual%20Studio%20Code%20has%20integrated,on%20the%20VS%20Code%20Marketplace.)

<h4 class="left">GitHub</h4>

- [GitHub collaboration workflow](https://guides.github.com/introduction/flow/)
- [GitHub & GitHub Pages tutorial](https://lab.github.com/githubtraining/introduction-to-github)
- Markdown [syntax cheatsheet](https://www.markdownguide.org/cheat-sheet/)


Content by Alice McGrath and licensed [cc-by-nc-sa](https://creativecommons.org/licenses/by-nc-sa/2.0/)


<!---
To run pandoc
pandoc -t revealjs git-hack/git-hub.md -o git-hack/git-hub.html -s --variable theme="alice"
--->

