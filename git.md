# git --help
**usage:**
git [--version] [--help] [-C <path>] [-c <name>=<value>]
    [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
	[-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
	[--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
	[--super-prefix=<path>] [--config-env=<name>=<envvar>]
	<command> [<args>]

**These are common Git commands used in various situations:**

- start a working area (see also: git help tutorial)
   - clone     --     Clone a repository into a new directory
   - init       --       Create an empty Git repository or reinitialize an existing one 
```example
 git clone https://github.com/lanhaner/funcool.git
 git init
 ```
- work on the current change (see also: git help everyday)
   - add         --      Add file contents to the index
   - mv           --     Move or rename a file, a directory, or a symlink 
   - restore      --   Restore working tree files
   - rm            --    Remove files from the working tree and from the index
   - sparse-checkout --  Initialize and modify the sparse-checkout
```example
git add git.txt
git mv git.txt
git rm git.txt
 ```

- examine the history and state (see also: git help revisions)
   - bisect      --    Use binary search to find the commit that introduced a bug
   - diff        --      Show changes between commits, commit and working tree, etc
   - grep      --      Print lines matching a pattern
   - log       --       Show commit logs
   - show      --     Show various types of objects
   - status     --     Show the working tree status
```example
git diff git.txt
git log
git show
git status
```
- grow, mark and tweak your common history
   - branch      --      List, create, or delete branches
   - commit     --       Record changes to the repository
   - merge       --      Join two or more development histories together
   - rebase     --       Reapply commits on top of another base tip
   - reset     --        Reset current HEAD to the specified state
   - switch      --      Switch branches
   - tag        --       Create, list, delete or verify a tag object signed with GPG

- collaborate (see also: git help workflows)
   - fetch      --      Download objects and refs from another repository
   - pull       --       Fetch from and integrate with another repository or a local branch
   - push       --     Update remote refs along with associated objects
```example
git push -u origin main
```

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

# add new file
```
git status
```
On branch main

Your branch is up to date with 'origin/main'.

Untracked files:

  (use "git add <file>..." to include in what will be committed)
  
  git.txt


nothing added to commit but untracked files present (use "git add" to track)

```
git add git.txt
git status
```
On branch main

Your branch is up to date with 'origin/main'.


Changes to be committed:

 (use "git restore --staged <file>..." to unstage)
 
 new file:   git.txt

```
git commit -m "git CLI"
```

E:\funcool>git commit -m "git CLI"

[main 5efed32] git CLI

 1 file changed, 53 insertions(+)
 
 create mode 100644 git.txt

```
git push -u origin main
```
Enumerating objects: 4, done.

Counting objects: 100% (4/4), done.

Delta compression using up to 6 threads

Compressing objects: 100% (3/3), done.

Writing objects: 100% (3/3), 1.32 KiB | 1.32 MiB/s, done.

Total 3 (delta 0), reused 0 (delta 0), pack-reused 0

To https://github.com/lanhaner/funcool.git

   91bc1a1..5efed32  main -> main
   
Branch 'main' set up to track remote branch 'main' from 'origin'.

# modify file
```
git status
```
On branch main

Your branch is up to date with 'origin/main'.

Changes not staged for commit:

  (use "git add <file>..." to update what will be committed)
  
  (use "git restore <file>..." to discard changes in working directory)
  
  modified:   git.txt

no changes added to commit (use "git add" and/or "git commit -a")
```
git diff git.txt
```
diff --git a/git.txt b/git.txt

index 57c437d..f44f6a5 100644

--- a/git.txt

+++ b/git.txt

@@ -9,23 +9,31 @@ usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]

 These are common Git commands used in various situations:

 start a working area (see also: git help tutorial)
 
-clone             Clone a repository into a new directory

+clone          Clone a repository into a new directory

*quit by letter 'q'*

```
git add git.txt
git commit -m "git CLI"
git push -u origin main
```

# delete file
```
git rm test.txt
git commit -m "remove test.txt"
git push -u origin main
```