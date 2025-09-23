# 1. Clonar repo de GitHub
git clone https://github.com/960-darkangel/DJANGO.git
cd DJANGO

# 2. Crear .gitignore
nano .gitignore   # (o notepad .gitignore si no tenés nano)
.gitignore recomendado
# --- Python ---
__pycache__/
*.py[cod]
*$py.class

# --- Entornos virtuales ---
env/
venv/
ENV/
*.pyo
*.pyd

# --- Archivos de base de datos (SQLite) ---
db.sqlite3

# --- Migraciones cacheadas ---
*/migrations/__pycache__/
*/migrations/*.pyc
*/migrations/*.pyo

# --- Archivos de Django ---
media/
staticfiles/

# --- Archivos locales ---
*.log
*.pot
*.env
*.ini
*.cfg

# --- IDEs y editores ---
.vscode/
.idea/
*.swp
*~

# --- Archivos de sistema ---
.DS_Store
Thumbs.db

git add .gitignore
git commit -m "Agregado .gitignore inicial"
git push origin main

# 3. Verificar versión de Python
python --version
# si no funciona, probá:
py --version

# 4. Crear entorno virtual
python -m venv env

# 5. Activar entorno virtual
# Opción A (Git Bash):
source env/Scripts/activate
# Opción B (cmd de Windows):
env\Scripts\activate.bat

# 6. Actualizar pip e instalar Django
python -m pip install --upgrade pip
python -m pip install django

# 7. Guardar dependencias en requirements.txt
pip freeze > requirements.txt

git add requirements.txt
git commit -m "Agregado requirements.txt"
git push origin main

# 8. Crear proyecto Django en la carpeta actual
django-admin startproject SO_i210 .

# 9. Crear una aplicación dentro del proyecto
python manage.py startapp mi_app

git add .
git commit -m "Creado proyecto Django con app inicial"
git push origin main


python manage.py runserver

