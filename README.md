<!DOCTYPE html>
<!--
	Git lab and reminders.
	Created on October, 2021.
  by siomara.com.br
-->
<html lang="en">

<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/js/bootstrap.bundle.min.js"></script>
</head>

<body>

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

  <h1>Welcome to my GIT lab and reminders collection!</h1>
  This repo was created from scratch with GIT and GITBASH to work as a lab so I can practice the instructions via
  command lines.

  <!-- What is Git in a nutshell -->
  <div class="container mt-3">
    <a href="#nutshell" class="btn btn-primary" data-bs-toggle="collapse">What is Git in a nutshell</a>
    <div id="nutshell" class="collapse">
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
    </div>
  </div>

  <!-- How Git works -->
  <div class="container mt-3">
    <a href="#howgitworks" class="btn btn-primary" data-bs-toggle="collapse">How Git works</a>
    <div id="howgitworks" class="collapse">
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
    </div>
  </div>

  <!-- Git Tutorial & Guide -->
  <div class="container mt-3">
    <a href="#gitguides" class="btn btn-primary" data-bs-toggle="collapse">Git Tutorial & Guide</a>
    <div id="gitguides" class="collapse">
      <p>
      <p>
        <a href="https://git-scm.com/docs/gittutorial"><img alt="">Tutorial</a>
        (https://git-scm.com/docs/gittutorial)
      </p>
      <p>
        <a href="https://github.com/git-guides/"><img alt="">Guides</a>
        (https://github.com/git-guides/)
      </p>
      </p>
    </div>
  </div>

  <!-- Installing Git -->
  <div class="container mt-3">
    <a href="#installinggit" class="btn btn-primary" data-bs-toggle="collapse">Installing Git</a>
    <div id="installinggit" class="collapse">
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
    </div>
  </div>

  <!-- Verify installation -->
  <div class="container mt-3">
    <a href="#verifyinstallation" class="btn btn-primary" data-bs-toggle="collapse">Verify installation by checking Git
      version</a>
    <div id="verifyinstallation" class="collapse">
      <p>
      <p>$ git --version</p>
      git version 2.33.0.windows.1
      </p>
    </div>
  </div>

  <!-- Check Git help -->
  <div class="container mt-3">
    <a href="#checkgithelp" class="btn btn-primary" data-bs-toggle="collapse">Check Git help</a>
    <div id="checkgithelp" class="collapse">
      <p>
      <p>$ git help</p>
      </p>
    </div>
  </div>

  <!-- Configure Git -->
  <div class="container mt-3">
    <a href="#configuregit" class="btn btn-primary" data-bs-toggle="collapse">Configure Git</a>
    <div id="configuregit" class="collapse">
      <p>
      <p>$ git config --global user.name "Siomara Cintia Pantarotto"</p>
      <p>$ git config --global user.email "siomarapantarotto@gmail.com"</p>
      <p>$ git config --global color.ui auto</p>
      <p>$ git config -l</p>
      </p>
    </div>
  </div>

  <!-- Initializing Git repository -->
  <div class="container mt-3">
    <a href="#initializinggitrepository" class="btn btn-primary" data-bs-toggle="collapse">Initializing Git
      repository</a>
    <div id="initializinggitrepository" class="collapse">
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
    </div>
  </div>

  <!-- Removing Git rpository -->
  <div class="container mt-3">
    <a href="#removinggitrepository" class="btn btn-primary" data-bs-toggle="collapse">Removing Git repository</a>
    <div id="removinggitrepository" class="collapse">
      <p>
      <p>
        $ ls -a<br />
        $ rm -rf .git<br />
        $ ls -a<br />
        $ git add<br />
        fatal: not a git repository (or any of the parent directories): .git<br />
        $ git init .<br />
        Initialized empty Git repository in D:/Users/Sioma/OneDrive/Área de Trabalho/git-memos/.git/
      </p>
      </p>
    </div>
  </div>

  <!-- Git add -->
  <div class="container mt-3">
    <a href="#guitadd" class="btn btn-primary" data-bs-toggle="collapse">Git add</a>
    <div id="guitadd" class="collapse">
      <p>
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
    </div>
  </div>

  <!-- Commits -->
  <div class="container mt-3">
    <a href="#commit" class="btn btn-primary" data-bs-toggle="collapse">Commits</a>
    <div id="commit" class="collapse">
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
    </div>
  </div>

  <!-- Amend commit messages -->
  <div class="container mt-3">
    <a href="#amendcommitmessages" class="btn btn-primary" data-bs-toggle="collapse">Amend commit messages</a>
    <div id="amendcommitmessages" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Git and Github -->
  <div class="container mt-3">
    <a href="#guitandgithub" class="btn btn-primary" data-bs-toggle="collapse">Git and Github</a>
    <div id="guitandgithub" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Create a GitHub repo -->
  <div class="container mt-3">
    <a href="#createaguitrepo" class="btn btn-primary" data-bs-toggle="collapse">Create a GitHub repo</a>
    <div id="createaguitrepo" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- SSH Keys Setup -->
  <div class="container mt-3">
    <a href="#sshkeyssetup" class="btn btn-primary" data-bs-toggle="collapse">SSH Keys setup</a>
    <div id="sshkeyssetup" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Git Push -->
  <div class="container mt-3">
    <a href="#guitpush" class="btn btn-primary" data-bs-toggle="collapse">Git push</a>
    <div id="guitpush" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Git Pull -->
  <div class="container mt-3">
    <a href="#guitpull" class="btn btn-primary" data-bs-toggle="collapse">Git pull</a>
    <div id="guitpull" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Understanding Branches -->
  <div class="container mt-3">
    <a href="#understandingbranches" class="btn btn-primary" data-bs-toggle="collapse">Understanding branches</a>
    <div id="understandingbranches" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Working with Branches -->
  <div class="container mt-3">
    <a href="#workingwithbranches" class="btn btn-primary" data-bs-toggle="collapse">Working with branches</a>
    <div id="workingwithbranches" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Main and Master are the same -->
  <div class="container mt-3">
    <a href="#mainandmasterarethesame" class="btn btn-primary" data-bs-toggle="collapse">Prefer MAIN rather than
      MASTER</a>
    <div id="mainandmasterarethesame" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Pull Requests -->
  <div class="container mt-3">
    <a href="#pullrequest" class="btn btn-primary" data-bs-toggle="collapse">Pull requests</a>
    <div id="pullrequest" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Merging and Pull Requests -->
  <div class="container mt-3">
    <a href="#mergingandpullrequests" class="btn btn-primary" data-bs-toggle="collapse">Merging and pull requests</a>
    <div id="mergingandpullrequests" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- The General Workflow -->
  <div class="container mt-3">
    <a href="#thegeneralworkflow" class="btn btn-primary" data-bs-toggle="collapse">The general workflow</a>
    <div id="thegeneralworkflow" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Conflicts -->
  <div class="container mt-3">
    <a href="#conflicts" class="btn btn-primary" data-bs-toggle="collapse">Conflicts</a>
    <div id="conflicts" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Merging Conflicts -->
  <div class="container mt-3">
    <a href="#mergingconflicts" class="btn btn-primary" data-bs-toggle="collapse">Merging conflicts</a>
    <div id="mergingconflicts" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Rebase -->
  <div class="container mt-3">
    <a href="#rebase" class="btn btn-primary" data-bs-toggle="collapse">Rebase</a>
    <div id="rebase" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Rebase recap -->
  <div class="container mt-3">
    <a href="#rebaserecap" class="btn btn-primary" data-bs-toggle="collapse">Rebase recap</a>
    <div id="rebaserecap" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

  <!-- Git clients -->
  <div class="container mt-3">
    <a href="#guitclients" class="btn btn-primary" data-bs-toggle="collapse">Git clients</a>
    <div id="guitclients" class="collapse">
      <p>
      <p>TODO</p>
      </p>
    </div>
  </div>

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

  <hr>

</body>

</html>
