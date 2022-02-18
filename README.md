<p align='center'>
  <img
    src="https://img.shields.io/badge/GitHub-Git/Git%20Bash-4183C4?style=for-the-badge&logo=github&logoColor=white" />&nbsp;&nbsp;
  <img
    src="https://img.shields.io/badge/Git%20via%20Git%20Bash-Under%20Construction-999999?style=for-the-badge&logo=git&logoColor=white" />&nbsp;&nbsp;
</p>

<p align='center'>
  <a href="https://git-scm.com/docs/gittutorial"><img alt=""
      src="https://user-images.githubusercontent.com/5893219/134832432-5eaa7a49-9727-4485-baeb-cd7a0deff034.png"></a>
</p>

# Welcome to my GIT reminders collection!

## Table of contents

- [Welcome to my GIT reminders collection!](#welcome-to-my-git-reminders-collection)
  - [Table of contents](#table-of-contents)
  - [General info](#general-info)
  - [What is Git in a nutshell](#what-is-git-in-a-nutshell)
  - [How Git works](#how-git-works)
  - [Git Tutorial and Guide](#git-tutorial-and-guide)
  - [Installing Git](#installing-git)
  - [Verify installation](#verify-installation)
  - [Check Git help](#check-git-help)
  - [Configure Git](#configure-git)
  - [Initializing Git repository](#initializing-git-repository)
  - [Removing Git repository](#removing-git-repository)
  - [Git add](#git-add)
  - [Commits](#commits)
  - [Amend commit messages](#amend-commit-messages)
  - [Git and Github](#git-and-github)
  - [Create a GitHub repo](#create-a-github-repo)
  - [SSH Keys Setup](#ssh-keys-setup)
  - [Git Push](#git-push)
  - [Git Pull](#git-pull)
  - [Understanding Branches](#understanding-branches)
  - [Working with Branches](#working-with-branches)
  - [Main and Master are the same](#main-and-master-are-the-same)
  - [Pull Requests](#pull-requests)
  - [Merging and Pull Requests](#merging-and-pull-requests)
  - [The General Workflow](#the-general-workflow)
  - [Conflicts](#conflicts)
  - [Merging Conflicts](#merging-conflicts)
  - [Rebase](#rebase)
  - [Rebase recap](#rebase-recap)
  - [Git clients](#git-clients)
  - [Thanks and how to contribute](#thanks-and-how-to-contribute)

## General info

This repo was created from scratch with GIT and GITBASH. Eventhough its content may not make much sense
to those who visit it, it is here that I cashe reminders when I need to use Git via command lines.

## What is Git in a nutshell

<p>
<ul>
  <li>Git is a commonly used <b>decentralized source code repository</b>.</li>
  <li><b>Created by the Linux creator Linus Torvalds</b> for the management of the Linux kernel source code.</li>
  <li>Whole services like GitHub and GitLab are based around it.</li>
  <li>Other free-to-use file version control systems (<b>VCS</b>):</li>
  <ul>
    <li><b>CVS</b> (Concurrent Versions System) – <text style="color:orange">First released</text></li>
    <li><b>SVN</b> (Apache Subversion) – <text style="color:orange">Second released</text></li>
    <li><b>Git</b> – <text style="color:orange">Third released</text></li>
    <li><b>Mercurial</b></li>
    <li><b>Bazaar</b> etc</li>
  </ul>
</ul>
</p>

## How Git works

<p>
<ul>
  <li>Git <b>handles content in snapshots, one for each commit</b>, and knows how to <b>apply or roll back the
      change sets
      between two snapshots</b>.</li>
  <li>Architecture:</li>
  <ul>
    <li><b><text style="color:orange">(local machine)</text> Working Directory</b> (Content)</li>
    - add to
    <li><b><text style="color:orange">(local machine)</text> Staging Area</b> (Index)</li>
    - commit to (a commit is basically a safe point)
    <li><b><text style="color:orange">(local machine)</text> Repository</b> (Commit History: Content [A], [B]…
      [N])</li>
    - push to
    <li><b><text style="color:orange">(remote servers)</text></b> Github, Gitlab, Bitbucket, AWS Code Commit etc
    </li>
  </ul>
</ul>
</p>

## Git Tutorial and Guide

<p>
  <a href="https://git-scm.com/docs/gittutorial"><img alt="">Tutorial</a>
  (https://git-scm.com/docs/gittutorial)
</p>
<p>
  <a href="https://github.com/git-guides/"><img alt="">Guides</a>
  (https://github.com/git-guides/)
</p>

## Installing Git

<p>
  <ul>
    <li>Git Installation for Mac and Windows users.</li>
    <a href="https://github.com/git-guides/install-git"><img alt="">https://github.com/git-guides/install-git</a>
    <br /><br />
    <li>Windows Users please install:</li>
    <ul>
      <li>
        GitBash
        <a href="https://gitforwindows.org/"><img alt="">https://gitforwindows.org/</a>
      </li>
      or
      <li>Cmder
        <a href="https://cmder.net/"><img alt="">https://cmder.net/</a>
      </li>
    </ul>
  </ul>
  </p>

## Verify installation

  <p>
  <mark>$ git --version</mark>
  git version 2.33.0.windows.1
  </p>

## Check Git help

<p><mark>$ git help</mark></p>

## Configure Git

<p>
  <mark>$ git config --global user.name "Siomara Cintia Pantarotto"</mark><br />
  <mark>$ git config --global user.email "siomarapantarotto@gmail.com"</mark><br />
  <mark>$ git config --global color.ui auto</mark><br />
  <mark>$ git config -l</mark><br />
</p>

## Initializing Git repository

<p>
  <p>Initializing with <b>git init .</b> is just for brand new projects, not existing ones.</p>
  <p>The <b>dot (.)</b> stands for the current directory.</p>
  $ ls
  $ cd desktop<br />
  $ ls<br />
  $ mkdir git-prompts<br />
  $ cd git-prompts<br />
  $ ls<br />
  <mark>$ git init .</mark><br />
  $ ls -a<br />
  </p>

## Removing Git repository

<p>
  $ ls -a<br />
  <mark>$ rm -rf .git</mark><br />
  $ ls -a<br />
  $ git add<br />
  fatal: not a git repository (or any of the parent directories): .git<br />
  $ git init .<br />
  Initialized empty Git repository in D:/Users/Sioma/OneDrive/Área de Trabalho/git-memos/.git/
</p>

## Git add

<p>
  $ git add
  Nothing specified, nothing added.
</p>
<p>
  $ ls -a
</p>
<p>
  $ touch index.html
  <br />$ touch index.js
  <br />$ touch main.css
</p>
<p>
  $ ls
  <br />index.html index.js main.css
</p>
<p>
  $ git status
  <br />On branch master
  <br />No commits yet
  <br />Untracked files:
  <br />(use "git add <file_name>..." to include in what will be committed)
    <br />index.html
    <br />index.js
    <br />main.css
</p>

## Commits

<p>
  A commit is basically a safe point.
<p>
  <br />$ git status
  <br />On branch master
  <br />No commits yet
  <br />Changes to be committed:
  <br />(use "git rm --cached <file>..." to unstage)
  <br />  new file: ../index.html
  <br />  new file: ../index.js
  <br />  new file: ../main.css
  <br />  new file: test.js
</p>
<p>$ cd ..</p>
<p>$ git status</p>
<p>$ git commit -m "bootstrap project"</p>
<p>$ git status</p>
<p>$ git log
<br/>  commit 178c5e3ae1d735eeee5469bfebd977f3eb8006f2 (HEAD -> master)
<br/>  Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>    Date: Sat Sep 25 00:29:54 2021 -0300

<br/>    bootstrap project

</p>
<p>
<br/>$ git show 178c5e3ae1d735eeee5469bfebd977f3eb8006f2
<br/>  commit 178c5e3ae1d735eeee5469bfebd977f3eb8006f2 (HEAD -> master)
<br/>  Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>    Date: Sat Sep 25 00:29:54 2021 -0300

<br/>    bootstrap project

<br/>    diff --git a/index.html b/index.html
<br/>    new file mode 100644
<br/>    index 0000000..e69de29
<br/>    diff --git a/index.js b/index.js
<br/>    new file mode 100644
<br/>    index 0000000..e69de29
<br/>    diff --git a/main.css b/main.css
<br/>    new file mode 100644
<br/>    index 0000000..e69de29
<br/>    diff --git a/test/test.js b/test/test.js
<br/>    new file mode 100644
<br/>    index 0000000..e69de29

</p>
<p>
$ vi index.js

i for insert and type:
<br/>console.log("Hello Git");
<br/>escape :wq
</p>

## Amend commit messages

<p>
User@HOST MINGW64 /desktop/git-memos (master)
<br />$ ls
<br />index.html  index.js  main.css  test/

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$ vi main.css

<br/>body {
<br/>}
<br/>~
<br/>~
<br/>~
<br/>~
<br/>~
<br/>~
<br/>~
<br/>main.css [unix] (09:21 25/09/2021) 2,1 All
<br/>:wq

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$ git status
<br/>On branch master
<br/>Changes not staged for commit:
<br/>(use "git add <file>..." to update what will be committed)
<br/>(use "git restore <file>..." to discard changes in working directory)
<br/>modified: main.css

<br/>no changes added to commit (use "git add" and/or "git commit -a")

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$ git add .
<br/>warning: LF will be replaced by CRLF in main.css.
<br/>The file will have its original line endings in your working directory

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$ git commit -m "gfhjdgsjdfgsjgfjgdjgdghgsg"
<br/>[master 7b71d8d] gfhjdgsjdfgsjgfjgdjgdghgsg
<br/>1 file changed, 2 insertions(+)

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$ git log
<br/>commit 7b71d8dcd4a73c07283297fd2f22a233fd3afc2b (HEAD -> master)
<br/>Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>Date: Sat Sep 25 10:20:49 2021 -0300

<br/>    gfhjdgsjdfgsjgfjgdjgdghgsg

<br/>commit 573500237a9e9e4c857bcd7f48d99b0cab0d22dc
<br/>Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>Date: Sat Sep 25 00:49:16 2021 -0300

<br/>    added console.log

<br/>commit 178c5e3ae1d735eeee5469bfebd977f3eb8006f2
<br/>Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>Date: Sat Sep 25 00:29:54 2021 -0300

<br/>    bootstrap project

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$ git commit --amend -m "added body{} in main.css"
<br/>[master 7e2596f] added body{} in main.css
<br/>Date: Sat Sep 25 10:20:49 2021 -0300
<br/>1 file changed, 2 insertions(+)

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$ git log
<br/>commit 7e2596f32bd99bb0c56f85d2ba1cbcc67131a45b (HEAD -> master)
<br/>Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>Date: Sat Sep 25 10:20:49 2021 -0300

<br/>    added body{} in main.css

<br/>commit 573500237a9e9e4c857bcd7f48d99b0cab0d22dc
<br/>Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>Date: Sat Sep 25 00:49:16 2021 -0300

<br/>    added console.log

<br/>commit 178c5e3ae1d735eeee5469bfebd977f3eb8006f2
<br/>Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
<br/>Date: Sat Sep 25 00:29:54 2021 -0300

<br/>    bootstrap project

<br/>User@HOST MINGW64 /desktop/git-memos (master)
<br/>$

</p>

## Git and Github

<p>TODO</p>

## Create a GitHub repo

<p>
<h2>…or create a new repository on the command line</h2>
<br/>echo "# git-prompts" >> README.md
<br/>git init
<br/>git add README.md
<br/>git commit -m "first commit"
<br/>git branch -M main
<br/>git remote add origin https://github.com/siomarapantarotto/git-prompts.git
<br/>git push -u origin main

<h2>…or push an existing repository from the command line</h2>
<br/>git remote add origin https://github.com/siomarapantarotto/git-prompts.git
<br/>git branch -M main
<br/>git push -u origin main

<h2>…or import code from another repository</h2>
<br/>You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
</p>

## SSH Keys Setup

<p>TODO</p>

## Git Push

<p>TODO</p>

## Git Pull

<p>TODO</p>

## Understanding Branches

<p>TODO</p>

## Working with Branches

<p>TODO</p>

## Main and Master are the same

<p>TODO</p>

## Pull Requests

<p>TODO</p>

## Merging and Pull Requests

<p>
<br />User@HOST ~ /desktop/git-prompts (main)
<br />$ ls
<br />README.md  index.html  index.js  main.css  main.go  test/

<br />User@HOST ~ /desktop/git-prompts (main)
<br />$ git log --oneline
<br />e9c8282 (HEAD -> main, origin/main) Update README.md
<br />f12e7b2 Update README.md
<br />27fdd14 Update README.md
<br />69993f9 added package main
<br />c62e7b2 Create README.md
<br />3982a93 added empty main function
<br />35376fe added console.log()
<br />742015e added body{}
<br />0591c35 fictitious bootstrap project
<br />a3e89fa added console.log()
<br />856c93c initial commit after clone issue during push to GitHub

<br />User@HOST ~ /desktop/git-prompts (main)
<br />$ git pull
<br />remote: Enumerating objects: 9, done.
<br />remote: Counting objects: 100% (9/9), done.
<br />remote: Compressing objects: 100% (5/5), done.
<br/>remote: Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
<br/>Unpacking objects: 100% (5/5), 1.34 KiB | 0 bytes/s, done.
<br/>From https://github.com/siomarapantarotto/git-prompts
<br/>e9c8282..4072369 main -> origin/main
<br/>Updating e9c8282..4072369
<br/>Fast-forward
<br/>README.md | 4 ++++
<br/>utils.js | 1 +
<br/>2 files changed, 5 insertions(+)
<br/>create mode 100644 utils.js

<br/>User@HOST ~ /desktop/git-prompts (main)
<br/>$ git log --oneline
<br/>4072369 (HEAD -> main, origin/main) Merge pull request #1 from siomarapantarotto/feature-a
<br/>c92dd30 Update README.md
<br/>e9c8282 Update README.md
<br/>f12e7b2 Update README.md
<br/>27fdd14 Update README.md
<br/>5351fe1 (origin/feature-a, feature-a) utils.js with TODO
<br/>69993f9 added package main
<br/>c62e7b2 Create README.md
<br/>3982a93 added empty main function
<br/>35376fe added console.log()
<br/>742015e added body{}
<br/>0591c35 fictitious bootstrap project
<br/>a3e89fa added console.log()
<br/>856c93c initial commit after clone issue during push to GitHub

<br/>User@HOST ~ /desktop/git-prompts (main)
<br/>$ git branch -d feature-a
<br/>Deleted branch feature-a (was 5351fe1).

<br/>User@HOST ~ /desktop/git-prompts (main)
<br/>$ git branch -a

<br/>- main
<br/>remotes/origin/feature-a
<br/>remotes/origin/main
</p>

## The General Workflow

<p>TODO</p>

## Conflicts

<p>TODO</p>

## Merging Conflicts

<p>TODO</p>

## Rebase

<p>TODO</p>

## Rebase recap

<p>TODO</p>

## Git clients

<p>TODO</p>

## Thanks and how to contribute

Thanks for viewing this repo! Contributions are more than welcome.

Feel free to contact me for more information.

<!-- FOOTER (Author / Visit My Online Resume / Download My PDF Resume) -->
<hr>
<p align='center'>
  <a href="#"><img
      src="https://img.shields.io/badge/author-%C2%A9%20Siomara%20Cintia%20Pantarotto.%20All%20rights%20reserved.-008080?style=social"></a>&nbsp;&nbsp;
  <a href="https://siomara.com.br/"><img
      src="https://img.shields.io/badge/visit-My Online Resume-008080?style=social"></a>&nbsp;&nbsp;
  <a href="https://siomara.com.br/ResumePANTAROTTO.pdf"><img
      src="https://img.shields.io/badge/download-My PDF Resume-008080?style=social"></a>
</p>
