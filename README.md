## Clonar el repositorio en local

cd '/c/Users/edm24/OneDrive/Documentos/Escuela/Semestre_9/Int Web/U1'

git clone https://github.com/EduardoMezaA/-iw2023ittepic

![1](https://github.com/EduardoMezaA/-iw2023ittepic/assets/127335310/098427ee-1221-4d07-9909-79c49c147ddb)

## Crear en tu repositorio local un documento README.md

cd '/c/Users/edm24/OneDrive/Documentos/Escuela/Semestre_9/Int Web/U1/-iw2023ittepic'

git add README.md

git status


## Agregar al README.md los comandos utilizados hasta ahora y hacer un commit inicial con el mensaje Initial commit

git config --global user.email edm2402@hotmail.com
git config --global user.name Eduardo_Meza

git config --list

git commit -m "Initial commit"

![2](https://github.com/EduardoMezaA/-iw2023ittepic/assets/127335310/fe4d0d0d-9f1e-4480-80cf-4ef0cc0cbb98)


## Subir los cambios al repositorio remoto
git push -u origin main

![3](https://github.com/EduardoMezaA/-iw2023ittepic/assets/127335310/e3b84738-1bc9-4cda-b33a-e7e646bab237)


### Crear en el repositorio local un fichero llamado privado.txt
touch privado.txt


### Crear en el repositorio local una carpeta llamada privada
mkdir privada


### Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git
touch .gitignore

![4](https://github.com/EduardoMezaA/-iw2023ittepic/assets/127335310/8e8476f1-a5c0-42b1-aa40-1b0c60819ffc)


### Añadir archivo 1.txt al repositorio local
touch 1.txt


## Crear un tag v0.1
git tag -a v0.1 -m "Version 0.1"

git push origin v0.1

git tag

![5](https://github.com/EduardoMezaA/-iw2023ittepic/assets/127335310/a5640ca7-47ce-42c4-9031-b57c61fb74cc)


## Subir los cambios al repositorio remoto
git add .

git commit -m "Cambios"

git push

![6](https://github.com/EduardoMezaA/-iw2023ittepic/assets/127335310/1846fffb-4e87-4b89-8e49-e6ec9fdaea45)


## Crear una tabla con la información de al menos 5 de tus compañeros de clase

| Nombre | Github |
|--------|--------|
| Mauricio  | https://github.com/Hombrux |
| Andres  | https://github.com/andrestian01 |
| Gustavo  | https://github.com/gsuvo |
| Ivan  | https://github.com/IvanRobles19 |
| Victor  | https://github.com/elVeector |

## Subir todos los archivos y cambios realizados al repositorio remoto

git add .

git commit -m "Actualiazcion de README"

git push -u origin main

![7](https://github.com/EduardoMezaA/-iw2023ittepic/assets/127335310/69d0c628-3696-410c-9726-90233d4054e2)



# PARTE 2

## Crear una rama v0.2 y posicionarse

git checkout -b v0.2


## Añadir archivo 2.txt en la rama v0.2

touch 2.txt


## Subir los cambios al repositorio remoto

git add 2.txt

git commit -m "Segundo archivo txt"

git push origin v0.2


## Posicionarse en la rama master. Hacer un merge de la rama v0.2 en la rama master

git checkout main

git merge v0.2

git push

## Merge con conflicto

git add 1.txt

git commit -m "1.txt mod"


### Posicionarse en la rama v0.2 y poner Adiós en el archivo 1.txt y hacer commit

git checkout v0.2

git add 1.txt

git commit -m "1.txt yeet"


### Posicionarse de nuevo en la rama master y hacer un merge con la rama v0.2

git checkout main

git merge v0.2


### Listar las ramas con merge y las ramas sin merge

git branch --merged

git branch --no-merged

### Arreglar conflicto anterior y hacer un commit

imagenxd

git add 1.txt

git commit -m "1.txt conflicto resuelto"

### Crear un tag v0.2

git tag -a v0.2

git push origin v0.2

### Borrar la rama v0.2

git branch -d v0.2

git push origin --delete v0.2

## Listar los distintos commits con sus ramas y sus tags

git log --all --decorate --oneline --graph
