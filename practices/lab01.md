# Discovering Git 🪐

## Lab 01

## Parte 1: Crear un proyecto de GoHugo.

1. Instalar [Go Hugo](https://gohugo.io/).
2. Puedes explorar los temas del sitio de Hugo. De momento usaremos el siguiente repo: [Paper Theme](https://github.com/adityatelange/hugo-PaperMod). Crea un fork de este repo en tu perfil de GitHub. Esto creará una copia para ti.
3. Crea un nuevo sitio de hugo por medio de la línea de comando: `hugo new site my_site_name`
4. Versiona tu proyecto con git, haz commit de todos los archivos creados por default, enlázalo y súbelo a un repo de GitHub.

## Parte 2: Enlazar repos mediante submódulos.

5. Agrega el fork que hiciste como un submódulo de git a tu repo. 

> git submodule add git@github.com:carlogilmar/hugo-PaperMod.git themes/hugo-PaperMod

6. Haz commit de los cambios, y súbelos a GitHub. Ahí podrás ver que ahora el repo de tu blog y el tema están enlazados.

## Parte 3: Levantar el proyecto.

7. En el directorio del tema, hay una carpeta llamada `exampleSite`, contiene un ejemplo de las configuraciones de ese tema. Copia todos esos archivos, y llévalos a la raíz de tu proyecto, sobreescribe los archivos tal cuál.

Nota: Bajar el siguiente repo y cambiarse al branch `exampleSite`: `https://github.com/adityatelange/hugo-PaperMod.git` (solo es necesario los archivos de configuración y de la carpeta content donde están los archivos de posts)

9. Verifica que el nombre del tema en la configuración sea el mismo nombre del directorio del tema.
10. Levanta el proyecto con: `hugo server`. Y podrías ver tu sitio en la url que te marcará Hugo.

## Parte 4: Modificar tu nuevo blog.

10. Limpia tu blog, agrega tu información personal, y comienza a agregarle tu propio contenido. Recuerda hacer commits y subirlos a GitHub.

## Parte 5: Despliegue.

11. Crea un repositorio en GitHub vacío, este será para levantar tu proyecto con GitHub Pages.
12. Agrega ese repo como un submódulo de git en tu repo de Hugo en el directorio `public`

> git submodule add git@github.com:carlogilmar/hugo-PaperMod.git public

13. Construye tu proyecto con Hugo: `hugo -D`, esto va a generar todos los archivos estáticos de tu blog en la carpeta `public`.
14. Entra a la carpeta public, realiza commit de todo lo que se agregó y súbelo a GitHub.
15. Activa GitHub Pages para ver tu proyecto.
