#CLONACIÓN DE REPOSITORIO DE DJANGO EN DEBIAN-TILIX

git clone https://github.com/960-darkangel/DJANGO.git

cd DJANGO

nano .gitignore(
# Entornos virtuales
env/
venv/
ENV/
*.pyc
__pycache__/
*.pyo
*.pyd
*.sqlite3

# Archivos de configuración locales
*.env
*.log
*.pot
*.py[cod]
*~ 
.DS_Store
.idea/
.vscode/

# Archivos de Django
db.sqlite3
/media/
staticfiles/

# Archivos de migraciones que no quieras subir (opcional, aunque muchos sí los suben)
*/migrations/__pycache__/
*/migrations/*.pyc
*/migrations/*.pyo

# Archivos de compilación / paquetes
*.egg
*.egg-info/
dist/
build/
.eggs/

# Archivos de testing/coverage
.coverage
.tox/
nosetests.xml
coverage.xml
*.cover
*.py,cover
.hypothesis/

# Archivos de Git
.gitignore
)

ls -a
./  ../  .git/  .gitignore

git add .gitignore

git branch
* main

git commit -m "main"
******* main

python --version
Python 3.12.5

python3 -m venv env

source env/bin/activate

python install django

python3 -m pip install django --upgrade pip

touch requeriments.txt

python3 -m pip frezze > requeriments-txt

django-admin startproject SO_i210

python3 -m pip install django

python3 manage.py startapp
