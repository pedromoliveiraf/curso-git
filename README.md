PS D:\Workspace\Bootcamp> git log
fatal: your current branch 'main' does not have any commits yet
PS D:\Workspace\Bootcamp> git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
PS D:\Workspace\Bootcamp> git add README.md
PS D:\Workspace\Bootcamp> git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

PS D:\Workspace\Bootcamp> git commit -m "1º commit - criando o README.md"
[main (root-commit) d44048b] 1º commit - criando o README.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
PS D:\Workspace\Bootcamp>
PS D:\Workspace\Bootcamp>
PS D:\Workspace\Bootcamp> git status
On branch main
nothing to commit, working tree clean
PS D:\Workspace\Bootcamp> git log
commit d44048bcca2e8b14c1376813a6037bec477e031a (HEAD -> main)
Author: Pedro M O Ferreira <pedromof28@gmail.com>
Date:   Sun May 4 21:55:39 2025 -0300

    1º commit - criando o README.md
PS D:\Workspace\Bootcamp> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\Workspace\Bootcamp> git add README.md
PS D:\Workspace\Bootcamp> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

PS D:\Workspace\Bootcamp> git commit -m "2º commit - alterando o README.md"
[main 377bcd4] 2º commit - alterando o README.md
 1 file changed, 1 insertion(+)
PS D:\Workspace\Bootcamp> git status
On branch main
nothing to commit, working tree clean
PS D:\Workspace\Bootcamp> git log
commit 377bcd484605131f45bb34c7dfba025f6a790246 (HEAD -> main)
Author: Pedro M O Ferreira <pedromof28@gmail.com>
Date:   Sun May 4 22:00:36 2025 -0300

    2º commit - alterando o README.md

commit d44048bcca2e8b14c1376813a6037bec477e031a
Author: Pedro M O Ferreira <pedromof28@gmail.com>
Date:   Sun May 4 21:55:39 2025 -0300

    1º commit - criando o README.md
PS D:\Workspace\Bootcamp> git log --pretty=online
fatal: invalid --pretty format: online
PS D:\Workspace\Bootcamp> git log --pretty=oneline
377bcd484605131f45bb34c7dfba025f6a790246 (HEAD -> main) 2º commit - alterando o README.md
d44048bcca2e8b14c1376813a6037bec477e031a 1º commit - criando o README.md
PS D:\Workspace\Bootcamp> git branch
* main
PS D:\Workspace\Bootcamp> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\Workspace\Bootcamp> git add README.md 
PS D:\Workspace\Bootcamp> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md

PS D:\Workspace\Bootcamp> git commit -m "3º commit"                     
[main 795f673] 3º commit
 1 file changed, 1 insertion(+)
PS D:\Workspace\Bootcamp> git status
On branch main
nothing to commit, working tree clean
PS D:\Workspace\Bootcamp> git branch
* main
PS D:\Workspace\Bootcamp> git log --pretty=oneline 
795f673f8c0c8254f62092ba2f51ded1c0aa3e85 (HEAD -> main) 3º commit
377bcd484605131f45bb34c7dfba025f6a790246 2º commit - alterando o README.md
d44048bcca2e8b14c1376813a6037bec477e031a 1º commit - criando o README.md
PS D:\Workspace\Bootcamp> git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
PS D:\Workspace\Bootcamp> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\Workspace\Bootcamp> git add .
PS D:\Workspace\Bootcamp> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   index.html

PS D:\Workspace\Bootcamp> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

PS D:\Workspace\Bootcamp> git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add
PS D:\Workspace\Bootcamp> git add .
PS D:\Workspace\Bootcamp> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   index.html

PS D:\Workspace\Bootcamp> git commit -m "4º commit - Adicionando o index.html"
[main aa1b348] 4º commit - Adicionando o index.html
 2 files changed, 14 insertions(+), 2 deletions(-)
 create mode 100644 index.html
PS D:\Workspace\Bootcamp> git status
On branch main
nothing to commit, working tree clean
PS D:\Workspace\Bootcamp> git log --pretty=oneline
aa1b348a936e364998e613b279c57d03e4fde092 (HEAD -> main) 4º commit - Adicionando o index.html
795f673f8c0c8254f62092ba2f51ded1c0aa3e85 3º commit
377bcd484605131f45bb34c7dfba025f6a790246 2º commit - alterando o README.md
d44048bcca2e8b14c1376813a6037bec477e031a 1º commit - criando o README.md
PS D:\Workspace\Bootcamp> git diff
diff --git a/README.md b/README.md
index 72b687a..f9ceacb 100644
--- a/README.md
+++ b/README.md
@@ -1,3 +1 @@
-Bliblibli
-Blebleble
-Blobloblo
\ No newline at end of file
+Blablabla
diff --git a/index.html b/index.html
index 86426d2..91aa841 100644
--- a/index.html
+++ b/index.html
@@ -6,6 +6,6 @@
     <title>Document</title>
 </head>
 <body>
-    Hello, world!
+    Hello, guys!
 </body>
 </html>
\ No newline at end of file
PS D:\Workspace\Bootcamp> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\Workspace\Bootcamp> git status
On branch main
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        deleted:    index.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\Workspace\Bootcamp> git add .
PS D:\Workspace\Bootcamp> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        deleted:    index.html

PS D:\Workspace\Bootcamp> git restore --staged README.md
PS D:\Workspace\Bootcamp> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

PS D:\Workspace\Bootcamp> git commit -m "5º commit - deletando o index.html"
[main 21a797b] 5º commit - deletando o index.html
 1 file changed, 11 deletions(-)
 delete mode 100644 index.html
PS D:\Workspace\Bootcamp> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\Workspace\Bootcamp> git log --pretty=oneline
21a797bbf2d5584832dc566cde17feb557e23b2d (HEAD -> main) 5º commit - deletando o index.html
aa1b348a936e364998e613b279c57d03e4fde092 4º commit - Adicionando o index.html
795f673f8c0c8254f62092ba2f51ded1c0aa3e85 3º commit
377bcd484605131f45bb34c7dfba025f6a790246 2º commit - alterando o README.md
d44048bcca2e8b14c1376813a6037bec477e031a 1º commit - criando o README.md
PS D:\Workspace\Bootcamp> git branch
* main
PS D:\Workspace\Bootcamp> "Vou mudar a minha branch para outra"
Vou mudar a minha branch para outra
PS D:\Workspace\Bootcamp> git branch -M main
PS D:\Workspace\Bootcamp> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\Workspace\Bootcamp> git branch
* main
PS D:\Workspace\Bootcamp> git remote add origin https://github.com/pedromoliveiraf/curso-git.git
PS D:\Workspace\Bootcamp> "O comando anterior serve para comunicar o git local que estamos nos comunicamos com o git remoto da URL indicada. Estamos 'conectando' o repositório local com o remoto"
O comando anterior serve para comunicar o git local que estamos nos comunicamos com o git remoto da URL indicada. Estamos 'conectando' o repositório local com o remoto
PS D:\Workspace\Bootcamp> git remote get-url
usage: git remote get-url [--push] [--all] <name>

    --[no-]push           query push URLs rather than fetch URLs
    --[no-]all            return all URLs

PS D:\Workspace\Bootcamp> git remote get-url origin
https://github.com/pedromoliveiraf/curso-git.git
PS D:\Workspace\Bootcamp> "o seguinte comando 'git remote get-url origin' mostra o endereço do repositório remoto"
o seguinte comando 'git remote get-url origin' mostra o endereço do repositório remoto
PS D:\Workspace\Bootcamp> git log --pretty=oneline                                                                        
21a797bbf2d5584832dc566cde17feb557e23b2d (HEAD -> main) 5º commit - deletando o index.html
aa1b348a936e364998e613b279c57d03e4fde092 4º commit - Adicionando o index.html
795f673f8c0c8254f62092ba2f51ded1c0aa3e85 3º commit
377bcd484605131f45bb34c7dfba025f6a790246 2º commit - alterando o README.md
d44048bcca2e8b14c1376813a6037bec477e031a 1º commit - criando o README.md
PS D:\Workspace\Bootcamp> "Agora é hora de enviarmos para o repositório remoto nossas alterações. Estou satisfeito com o que foi feito, logo, vamos enviar usando o comando 'git push'"
Agora é hora de enviarmos para o repositório remoto nossas alterações. Estou satisfeito com o que foi feito, logo, vamos enviar usando o comando 'git push'
PS D:\Workspace\Bootcamp> "Ao usar esse comando, na sua primeira vez, precisamos mandar assim: 'git -u origin main', dessa forma estamos indicando para qual local vamos fazer o envio desses commits, indicando que vamos mandar para o origin da URL, na branch main (no exemplo)"
Ao usar esse comando, na sua primeira vez, precisamos mandar assim: 'git -u origin main', dessa forma estamos indicando para qual local vamos fazer o envio desses commits, indicando que vamos mandar para o origin da URL, na branch main (no exemplo)
PS D:\Workspace\Bootcamp> "Ao usar esse comando, na sua primeira vez, precisamos mandar assim: 'git push -u origin main', dessa forma estamos indicando para qual local vamos fazer o envio desses commits, indicando que vamos mandar para o origin da URL, na branch main (no exemplo)"                        
Ao usar esse comando, na sua primeira vez, precisamos mandar assim: 'git push -u origin main', dessa forma estamos indicando para qual local vamos fazer o envio desses commits, indicando que vamos mandar para o origin da URL, na branch main (no exemplo)
PS D:\Workspace\Bootcamp> git push -u origin main
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 20 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (15/15), 1.37 KiB | 700.00 KiB/s, done.
Total 15 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/pedromoliveiraf/curso-git.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS D:\Workspace\Bootcamp> git log --pretty=oneline                                                                        
21a797bbf2d5584832dc566cde17feb557e23b2d (HEAD -> main, origin/main) 5º commit - deletando o index.html                   
aa1b348a936e364998e613b279c57d03e4fde092 4º commit - Adicionando o index.html
795f673f8c0c8254f62092ba2f51ded1c0aa3e85 3º commit
377bcd484605131f45bb34c7dfba025f6a790246 2º commit - alterando o README.md
d44048bcca2e8b14c1376813a6037bec477e031a 1º commit - criando o README.md
PS D:\Workspace\Bootcamp> 