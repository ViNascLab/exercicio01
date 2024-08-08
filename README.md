<pre>
 
 --------------
| EXERCICIO 01 |
 --------------
Vinicius Ferreira do Nascimento
RA 1802295


<b>A) No working dir, executar o comando: echo 01 > arquivo.txt</b>
    @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 01 > arquivo.txt

 
<b>B) Adicionar o arquivo no staging e conferir o status</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
  On branch main
  
  No commits yet
  
  Changes to be committed:
    (use "git rm --cached <file>..." to unstage)
          new file:   arquivo.txt
     
<b>C) Commitar o arquivo do staging com a descrição "git add example - arquivo.txt“</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add example - arquivo.txt"
  [main (root-commit) 440eaf9] git add example - arquivo.txt
   1 file changed, 1 insertion(+)
   create mode 100644 arquivo.txt

     
<b>D) Sobrescrever o conteúdo do arquivo.txt: echo 02 > arquivo.txt</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 02 > arquivo.txt

     
<b>E) Verificar o diffing no arquivo</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
  diff --git a/arquivo.txt b/arquivo.txt
  index 8a0f05e..9e22bcb 100644
  --- a/arquivo.txt
  +++ b/arquivo.txt
  @@ -1 +1 @@
  -01
  +02

     
<b>F) Adicionar novamente o arquivo no staging e conferir o status</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
  On branch main
  Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
          modified:   arquivo.txt

     
<b>G) Verificar o diffing no arquivo</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff arquivo.txt

     
<b>H) Sobrescrever o conteúdo do arquivo.txt: echo 03 > arquivo.txt</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 03 > arquivo.txt

     
<b>I) Verificar o diffing no arquivo</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff arquivo.txt
    diff --git a/arquivo.txt b/arquivo.txt
    index 9e22bcb..75016ea 100644
    --- a/arquivo.txt
    +++ b/arquivo.txt
    @@ -1 +1 @@
    -02
    +03

     
<b>J) Fazer o restore do arquivo da área de staging e verificar o status</b>
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore --staged arquivo.txt
  @ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")

   
<b>K) Realizar o commit do arquivo e verificar o log</b>
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m arquivo.txt 
[main 5437956] arquivo.txt
 1 file changed, 1 insertion(+), 1 deletion(-)

   
<b>L) Adicionar um arquivo gitignore com o seguinte conteúdo: *.txt</b>
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ vi .gitignore
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m .
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add .gitignore 
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m .
[main a8761d6] .
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore



   
<b>M) Criar um arquivo novo.txt e verificar o status</b>
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo > novo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
nothing to commit, working tree clean



 ------------------------------
| - Output de toda a atividade: |
 ------------------------------

@ViNascLab ➜ /workspaces/codespaces-blank $ git config --global user.name "Vinicius Nascimento"
@ViNascLab ➜ /workspaces/codespaces-blank $ git config --global user.email "vinicius.nascimento@aluno.faculdadeimpacta.com.br"
@ViNascLab ➜ /workspaces/codespaces-blank $ mkdir exercicio01
@ViNascLab ➜ /workspaces/codespaces-blank $ cd exercicio01/
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 $ ls
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 $ git init
Initialized empty Git repository in /workspaces/codespaces-blank/exercicio01/.git/
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ ls
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cd .git/
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ ls
HEAD  branches  config  description  hooks  info  objects  refs
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ ls -a
.  ..  HEAD  branches  config  description  hooks  info  objects  refs
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ git status
fatal: this operation must be run in a work tree
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ cd ..
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 01 > arquivo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add example - arquivo.txt“
> 
> ^C
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add example - arquivo.txt"
[main (root-commit) 440eaf9] git add example - arquivo.txt
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 02 > arquivo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff arquivo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 03 > arquivo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore --staged arquivo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+03
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m arquivo.txt 
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m arquivo.txt 
[main 5437956] arquivo.txt
 1 file changed, 1 insertion(+), 1 deletion(-)
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ vi .gitignore
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo > novo.txt
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m .
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add .gitignore 
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m .
[main a8761d6] .
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
nothing to commit, working tree clean
@ViNascLab ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 

</pre>
