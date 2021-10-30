# Welcome to my GIT lab and reminders collection!

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

## Table of contents
* [General info](#general-info)
* [What is Git in a nutshell](#what-is-Git-in-a-nutshell)
* [How Git works](#how-git-works)
* [Git Tutorial and Guide](#git-tutorial-and-Guide)
* [Installing Git](#installing-git)
* [Verify installation](#verify-installation)
* [Check Git help](#check-git-help)
* [Configure Git](#configure-git)
* [Initializing Git repository](#initializing-git-repository)
* [Removing Git repository](#removing-git-repository)
* [Git add](#git-add)
* [Commits](#commits)
* [Amend commit messages](#amend-commit-messages)
* [Git and Github](#git-and-github)
* [Create a GitHub repo](#create-a-github-repo)
* [SSH Keys Setup](#ssh-keys-setup)
* [Git Push](#git-push)
* [Git Pull](#git-pull)
* [Understanding Branches](#understanding-branches)
* [Working with Branches](#working-with-branches)
* [Main and Master are the same](#main-and-master-are-the-same)
* [Pull Requests](#pull-requests)
* [Merging and Pull Requests](#merging-and-pull-requests)
* [The General Workflow](#the-general-workflow)
* [Conflicts](#conflicts)
* [Merging Conflicts](#merging-conflicts)
* [Rebase](#rebase)
* [Rebase recap](#rebase-recap)
* [Git clients](#git-clients)
* [Thanks and how to contribute](#thanks-and-how-to-contribute)


## General info
This repo was created from scratch with GIT and GITBASH to work as a lab. 
Even though its content may not make much sense to those who visit it, it is here that I cashe reminders to practice the instructions via
command lines.


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
<a href="#verifyinstallation" class="btn btn-primary" data-bs-toggle="collapse">Verify installation by checking Git
  version</a>
<div id="verifyinstallation" class="collapse">
  <p>
  <p>$ git --version</p>
  git version 2.33.0.windows.1
  </p>


## Check Git help
<p>$ git help</p>


## Configure Git
<p>
  <p>$ git config --global user.name "Siomara Cintia Pantarotto"</p>
  <p>$ git config --global user.email "siomarapantarotto@gmail.com"</p>
  <p>$ git config --global color.ui auto</p>
  <p>$ git config -l</p>
  </p>


## Initializing Git repository
<p>
  <p>Initializing with <b>git init .</b> is just for brand new projects, not existing ones.</p>
  <p>The <b>dot (.)</b> stands for the current directory.</p>
  $ ls<br />
  $ cd desktop<br />
  $ ls<br />
  $ mkdir git-prompts<br />
  $ cd git-prompts<br />
  $ ls<br />
  $ git init .<br />
  $ ls -a<br />
  </p>


## Removing Git repository
<p>
  $ ls -a<br />
  $ rm -rf .git<br />
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
  $ git status
  On branch master
  No commits yet
  Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
    new file: ../index.html
    new file: ../index.js
    new file: ../main.css
    new file: test.js
</p>
<p>$ cd ..</p>
<p>$ git status</p>
<p>$ git commit -m "bootstrap project"</p>
<p>$ git status</p>
<p>$ git log
  commit 178c5e3ae1d735eeee5469bfebd977f3eb8006f2 (HEAD -> master)
  Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
    Date: Sat Sep 25 00:29:54 2021 -0300

    bootstrap project
</p>
<p>$ git show 178c5e3ae1d735eeee5469bfebd977f3eb8006f2
  commit 178c5e3ae1d735eeee5469bfebd977f3eb8006f2 (HEAD -> master)
  Author: SIOMARA CINTIA PANTAROTTO <siomarapantarotto@gmail.com>
    Date: Sat Sep 25 00:29:54 2021 -0300

    bootstrap project

    diff --git a/index.html b/index.html
    new file mode 100644
    index 0000000..e69de29
    diff --git a/index.js b/index.js
    new file mode 100644
    index 0000000..e69de29
    diff --git a/main.css b/main.css
    new file mode 100644
    index 0000000..e69de29
    diff --git a/test/test.js b/test/test.js
    new file mode 100644
    index 0000000..e69de29
</p>
<p>$ vi index.js

  i for insert and type:
  console.log("Hello Git");
  escape :wq
</p>
<p></p>
</p>


## Amend commit messages
<p>TODO</p>


## Git and Github
<p>TODO</p>


## Create a GitHub repo
<p>TODO</p>


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
<p>TODO</p>


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
