# git-practice
Added a hello.txt file throught CMD
``
Microsoft Windows [Version 10.0.26100.4061]
(c) Microsoft Corporation. All rights reserved.

C:\Users\dhars>git
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
           [--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
           [--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   restore    Restore working tree files
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   diff       Show changes between commits, commit and working tree, etc
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   backfill   Download missing objects in a partial clone
   branch     List, create, or delete branches
   commit     Record changes to the repository
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   reset      Reset current HEAD to the specified state
   switch     Switch branches
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

C:\Users\dhars>git --version
git version 2.48.1.windows.1

C:\Users\dhars>git config --global user.name "Your Name"

C:\Users\dhars>git config --global user.email "youremail@example.com"

C:\Users\dhars>git config --global user.name "Dharshinisri G"

C:\Users\dhars>git config --global user.email "dharshinisrigajendran@gmail.com"

C:\Users\dhars>git clone https://github.com/Dharshinisri-G/git-practice
Cloning into 'git-practice'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

C:\Users\dhars>cd git-practice

C:\Users\dhars\git-practice>echo "Hello Git!" > hello.txt

C:\Users\dhars\git-practice>git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hello.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\dhars\git-practice>git add hello.txt

C:\Users\dhars\git-practice>git commit -m "Added hello.txt"
[main 6cdc2c6] Added hello.txt
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt

C:\Users\dhars\git-practice>git push origin main
info: please complete authentication in your browser...
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Dharshinisri-G/git-practice
   488c1d2..6cdc2c6  main -> main

C:\Users\dhars\git-practice>git pull origin main
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 976 bytes | 88.00 KiB/s, done.
From https://github.com/Dharshinisri-G/git-practice
 * branch            main       -> FETCH_HEAD
   6cdc2c6..c79990d  main       -> origin/main
Updating 6cdc2c6..c79990d
Fast-forward
 README.md | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\dhars\git-practice>
``

Command	 & Purpose
git clone <url>	Copy remote repo locally
git status	Check file changes
git add <file>	Stage file for commit
git commit -m "msg"	Commit staged files
git push origin main	Upload commits to GitHub
git pull origin main	Download latest changes
