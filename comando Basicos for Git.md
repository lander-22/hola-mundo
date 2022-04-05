# Comandos basicos Git
------------
- Variables de configuración
- Repositorios remotos
- Confirmaciones
- Ramificaciones
- Etiquetas
------------
## Variables de configuración
| Descripción  |  comando |
| ------------ | ------------ |
|Enumera todas las variables de configuración.|`git config --list`|
|Muestra únicamente las variables de configuración locales.| `git config --local -l` |
|Muestra únicamente las variables de configuración del sistema.| `git config --system -l`|
|Muestra únicamente las variables de configuración globales.| `git config --global -l` |
|Establece una configuración variable en el archivo de configuración especificado. | ` git config [--local  --global  --system] variable-name variable-value ` |
|Establece el nombre de ramificación predeterminada enprincipalpara todos los repositorios locales cuando se realiza una confirmación inicial en un repositorio que aún no tiene una rama predeterminada. | `git config --global init.defaultBranch main` |
|Edita un archivo de configuración directamente. También se puede utilizar para detectar la ubicación de un archivo de configuración concreto. Para salir del modo de edición, normalmente escribe :q (para salir sin guardar los cambios) o :wq (para guardar los cambios y salir) y, a continuación, pulsa Intro.| `git config [--local  --global --system] --edit`|

### Comandos Principales
- **`git clone <nameRepo>`**  : clonar los archivos del repositorio en github del respectivo brach o master(main).
- **`git fetch `**  :  para actualizar los archivos del brach recuerdo.
- **`git pull origin main `**  :
- **`git push origin main `**  :

### Comandos for Branch 

- **`git branch <nameNewBranch> `**  : si escribes sin el nombre del nuevo branch te listara los branches actuales , sino te creara uno nuevo con el nombre q le especifiques.
- **`git  checkout <namebranch>`**  : Es para moverse a un branch en especifico.
- **`git commit -am "mensaje de cambios" `**  : es para guardar cambios localmente mas no subirlos al branch.
- **`git  push origin <name branch>`**  :
- **`git checkout -b <namebranch> `**  : crea nuevo branch y te mueve automaticamente hacia el es la union de comandos 1 y 2 de esta lista.


