# Clona el repositorio y navega a él
git clone https://github.com/tu-usuario/tu-repositorio.git
cd tu-repositorio

# Crea y cámbiate a la nueva rama
# git branch feature-branch y git checkout feature-branch 
git checkout -b feature-branch

# Realiza algunos cambios y haz commit
echo "Algunos cambios" >> archivo.txt
git add archivo.txt
git commit -m "Agrega cambios en feature-branch"

# Cambia a la rama main
git checkout main

# Fusiona la rama feature-branch en main
git merge feature-branch

# Resuelve conflictos si los hay
# (Edita archivos, añade y haz commit)
git add archivo-con-conflicto.txt
git commit -m "Resuelve conflictos de merge"

# Borra la rama feature-branch si ya no es necesaria
git branch -d feature-branch
