#CLONACIÓN DE REPOSITORIO DE DJANGO EN DEBIAN-TILIX

git clone https://github.com/960-darkangel/DJANGO.git

cd DJANGO

nano .gitignore

ls -a
./  ../  .git/  .gitignore

git add .gitignore

git branch
* main

chicos@DESKTOP-VBRVOOB MINGW64 ~/DJANGO (main)
$ git cmmit -m "main"
git: 'cmmit' is not a git command. See 'git --help'.

$ git commit -m "main"
******* main

$ python --version
Python 3.12.5

$ python3 -m venv env

$ source env/bin/activate
