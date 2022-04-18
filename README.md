# Questão 1
https://github.com/rogeriokotsubo/my_first_steps

# Questão 2
roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub
$ mkdir my_first_steps

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub
$ cd my_first_steps

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps
$ git init
Initialized empty Git repository in D:/RogerioK/GitHub/my_first_steps/.git/

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (master)
$ git remote add origin git@github.com:rogeriokotsubo/my_first_steps.git

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (master)
$ git checkout -b main
Switched to a new branch 'main'

# Questão 3
roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ touch ola_mundo.txt

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ ls
ola_mundo.txt

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ vim ola_mundo.txt

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ola_mundo.txt

nothing added to commit but untracked files present (use "git add" to track)

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git add ola_mundo.txt
warning: LF will be replaced by CRLF in ola_mundo.txt.
The file will have its original line endings in your working directory

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git commit -m "adicionando ola_mundo ao repositório"
[main (root-commit) 9caf92f] adicionando ola_mundo ao repositório
 1 file changed, 2 insertions(+)
 create mode 100644 ola_mundo.txt

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git status
On branch main
nothing to commit, working tree clean

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 287 bytes | 287.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:rogeriokotsubo/my_first_steps.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

# Questão 4
roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ touch .gitignore

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ ls .gitignore
.gitignore

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ touch serei_ignorado.txt

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ vim serei_ignorado.txt

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ vim .gitignore

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git add .
warning: LF will be replaced by CRLF in .gitignore.
The file will have its original line endings in your working directory

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore


roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git commit
[main bbc5830] Adicionando .gitignore
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore

roger@DESKTOP-UP9LQBJ MINGW64 /d/RogerioK/GitHub/my_first_steps (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 313.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:rogeriokotsubo/my_first_steps.git
   9caf92f..bbc5830  main -> main
