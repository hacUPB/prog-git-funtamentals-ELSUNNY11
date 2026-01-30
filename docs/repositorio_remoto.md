# REPOSITORIO REMOTO GITHUB

1) Crear el repositorio remoto en GitHub

En GitHub, ve a New repository.

Ponle nombre (ideal: el mismo que tu carpeta local).

Elige Public o Private.

Recomendación para evitar líos:

Si ya tienes archivos y commits localmente, crea el repo VACÍO (sin README, sin .gitignore, sin licencia).

Si quieres que GitHub te cree README, también se puede, pero luego tendrás que hacer pull antes del primer push.

Al final, GitHub te mostrará una URL tipo:

HTTPS: https://github.com/USUARIO/REPO.git

SSH: git@github.com:USUARIO/REPO.git

2) Crear/confirmar tu repositorio local

En tu carpeta del proyecto:

cd ruta/a/tu/proyecto
git init


Verifica:

git status

3) Hacer tu primer commit (si no lo tienes)

Agrega archivos:

git add .


Crea commit:

git commit -m "Primer commit"


Si te dice que falta configurar usuario/correo:

git config --global user.name "Tu Nombre"
git config --global user.email "tucorreo@algo.com"

4) Conectar el local con el remoto (remote “origin”)

Agrega el remoto:

git remote add origin https://github.com/USUARIO/REPO.git


Comprueba que quedó bien:

git remote -v

5) Subir tu rama al remoto (primer push)

Hoy normalmente la rama se llama main. Confirma:

git branch


Si tu rama se llama master y quieres usar main:

git branch -M main


Ahora sí, sube y deja la rama “trackeada”:

git push -u origin main


Listo: desde ahí, los siguientes pushes suelen ser solo:

git push

6) Sincronizar cambios en ambos sentidos
Traer cambios del remoto (sin subir nada)
git pull

Subir tus cambios locales
git add .
git commit -m "Mensaje"
git push
