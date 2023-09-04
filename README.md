# Clonar el repositorio en local

cd '/c/Users/edm24/OneDrive/Documentos/Escuela/Semestre_9/Int Web/U1'

git clone https://github.com/EduardoMezaA/-iw2023ittepic

# Crear en tu repositorio local un documento README.md

cd '/c/Users/edm24/OneDrive/Documentos/Escuela/Semestre_9/Int Web/U1/-iw2023ittepic'

git add README.md

git status

# Agregar al README.md los comandos utilizados hasta ahora y hacer un
# commit inicial con el mensaje Initial commit

git config --global user.email edm2402@hotmail.com
git config --global user.name Eduardo_Meza

git config --list

git commit -m "Initial commit"

# Subir los cambios al repositorio remoto
git push -u origin main

# Crear en el repositorio local un fichero llamado privado.txt
touch privado.txt

# Crear en el repositorio local una carpeta llamada privada
mkdir privada

# Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git
touch .gitignore

# Añadir archivo 1.txt al repositorio local
touch 1.txt

# Crear un tag v0.1
git tag -a v0.1 -m "Version 0.1"

git tag

# Subir los cambios al repositorio remoto
git add .

git commit -m "Cambios"

git push


| Nombre | Github |
|--------|--------|
| Mauricio  | https://github.com/Hombrux |
| Andres  | https://github.com/andrestian01 |
| Gustavo  | https://github.com/gsuvo |
| Ivan  | https://github.com/IvanRobles19 |
| Victor  | https://github.com/elVeector |

