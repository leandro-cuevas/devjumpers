REPOSITORIO DEVJUMPERS


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github
$ git clone https://github.com/leandro-cuevas/devjumpers.git
Cloning into 'devjumpers'...
warning: You appear to have cloned an empty repository.

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github
$ cd devjumpers


README


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ touch README.md

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git add .


COMMIT INICIAL


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git commit -m "commit inicial"
[main (root-commit) e6ad68a] commit inicial
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md


PUSH INICIAL


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 219 bytes | 219.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/leandro-cuevas/devjumpers.git
 * [new branch]      main -> main


IGNORAR ARCHIVOS


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ touch privado.txt

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ mkdir privada

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ touch .gitignore

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ echo "privad*" >.gitignore

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git add .
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git commit -m "Se creó .gitignore"
[main ec1e9c9] Se creó .gitignore
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/leandro-cuevas/devjumpers.git
   e6ad68a..ec1e9c9  main -> main

COMENTARIO: Al momento de crear .gitignore se escribió "privad*" con un asterístico, ya que esto lo que hace es ignorar todo lo que comience con lo que uno haya escrito,
en este caso "privad" por lo cual aplicará para la carpeta como para el archivo .txt


AGREGAR ARCHIVO 1.TXT


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ touch 1.txt


CREAR RAMA V0.2


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git branch v0.2

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git checkout v0.2
Switched to branch 'v0.2'


AÑADIR ARCHIVO 2.TXT


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ touch 2.txt

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git add .


CREAR RAMA REMOTA V0.2


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git commit -m "Se creó rama v0.2"
[v0.2 0ac3dd1] Se creó rama v0.2
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 1.txt
 create mode 100644 2.txt

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git push
fatal: The current branch v0.2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin v0.2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git push --set-upstream origin v0.2
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 298 bytes | 298.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'v0.2' on GitHub by visiting:
remote:      https://github.com/leandro-cuevas/devjumpers/pull/new/v0.2
remote:
To https://github.com/leandro-cuevas/devjumpers.git
 * [new branch]      v0.2 -> v0.2
branch 'v0.2' set up to track 'origin/v0.2'.


MERGE DIRECTO


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git merge v0.2
Updating ec1e9c9..0ac3dd1
Fast-forward
 1.txt | 0
 2.txt | 0
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 1.txt
 create mode 100644 2.txt


MERGE CON CONFLICTO


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ echo "Hola" > 1.txt

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git add .
warning: in the working copy of '1.txt', LF will be replaced by CRLF the next time Git touches it

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git commit -m "Se agregó Hola en 1.txt"
[main 58fdac4] Se agregó Hola en 1.txt
 1 file changed, 1 insertion(+)

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git checkout v0.2
Switched to branch 'v0.2'
Your branch is up to date with 'origin/v0.2'.

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ echo "Adiós"> 1.txt

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git add .
warning: in the working copy of '1.txt', LF will be replaced by CRLF the next time Git touches it

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git commit m- "Se agregó Adiós en 1.txt"
error: pathspec 'm-' did not match any file(s) known to git
error: pathspec 'Se agregó Adiós en 1.txt' did not match any file(s) known to git

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git commit -m "Se agregó adiós en 1.txt"
[v0.2 5b61a2f] Se agregó adiós en 1.txt
 1 file changed, 1 insertion(+)

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (v0.2)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git merge v0.2
Auto-merging 1.txt
CONFLICT (content): Merge conflict in 1.txt
Automatic merge failed; fix conflicts and then commit the result.


LISTADO DE RAMAS


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main|MERGING)
$ git branch --merged
* main

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main|MERGING)
$ git branch --no-merged
  v0.2


ARREGLAR CONFLICTO


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main|MERGING)
$ git add .

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main|MERGING)
$ git commit -m "Se resolvieron los conflictos en 1.txt"
[main 71567a8] Se resolvieron los conflictos en 1.txt


BORRAR RAMA


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git branch -d v0.2
warning: not deleting branch 'v0.2' that is not yet merged to
         'refs/remotes/origin/v0.2', even though it is merged to HEAD.
error: The branch 'v0.2' is not fully merged.
If you are sure you want to delete it, run 'git branch -D v0.2'.

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git branch -D v0.2
Deleted branch v0.2 (was 5b61a2f).

Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git push
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 928 bytes | 464.00 KiB/s, done.
Total 9 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/leandro-cuevas/devjumpers.git
   ec1e9c9..71567a8  main -> main


LISTADO DE CAMBIOS


Leandro@DESKTOP-AOCAB70 MINGW64 /d/Documentos/GIT-github/devjumpers (main)
$ git log --oneline --decorate --all --graph
*   71567a8 (HEAD -> main, origin/main) Se resolvieron los conflictos en 1.txt
|\
| * 5b61a2f (d-) Se agregó adiós en 1.txt
* | 58fdac4 Se agregó Hola en 1.txt
|/
* 0ac3dd1 (origin/v0.2) Se creó rama v0.2
* ec1e9c9 Se creó .gitignore
* e6ad68a commit inicial


CUENTA DE GITHUB

Cambié mi foto de perfil y activé la debole autentificación


USO SOCIAL DE GITHUB

Seguí a mis compañeros de curso en la plataforma.


CREAR UNA TABLA


    NOMBRE                        GITHUB

María Arteaga           https://github.com/maryjse

Marcelo Taborda         https://github.com/Marcelo-Taborda

Lourdes Ávalos          https://github.com/LouAvalos

Damián Coronel          https://github.com/Damsh-bit

Camila Ríos             https://github.com/camilarios01


COLABORADORES


Invité a Enzo Franco a colaborar en mi repositorio.