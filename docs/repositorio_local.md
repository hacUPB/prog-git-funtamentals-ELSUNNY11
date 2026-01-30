# REPOSITORIO LOCAL

## Paso 1: Abrir la terminal en tu proyecto

Primero entra a la carpeta donde estará tu proyecto:

cd ruta/del/proyecto


Si la carpeta no existe, créala:

mkdir mi_proyecto
cd mi_proyecto

### Paso 2: Inicializar el repositorio

Dentro de la carpeta ejecuta:

git init


Esto:

Crea una carpeta oculta llamada .git/

Convierte la carpeta en un repositorio

Activa el control de versiones

Verás algo como:

Initialized empty Git repository...

#### Paso 3: Revisar el estado

Para comprobar que Git está funcionando:

git statusI


Muestra:

Archivos sin seguimiento.

Cambios pendientes.

Rama actual.

##### Paso 4: Agregar archivos al repositorio

Crea un archivo (por ejemplo):

touch README.md


Luego agrégalo:

git add README.md


O todos:

git add .

###### Paso 5: Hacer el primer commit

Guarda los cambios con:

git commit -m "Primer commit"

![img1](../images/REPO%20LOCAL.png)



