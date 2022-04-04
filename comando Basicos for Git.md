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
