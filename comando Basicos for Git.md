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
- **`git fetch `**  :  para actualizar los archivos del brach recuerdo, se debe de hacer antes del `git pull origin <namebranch>`.
- **`git pull origin <namebranch> `**  : Es para cargar archivos del remoto al local independiente del branch en el q estes.
- **`git push origin <namebranch> `**  : Es para subir un commit al brach elegido basicamente es lo contrario del pull , del local al remoto.

### Comandos for Branch 

- **`git branch <nameNewBranch> `**  : si escribes sin el nombre del nuevo branch te listara los branches actuales , sino te creara uno nuevo con el nombre q le especifiques.
- **`git  checkout <namebranch>`**  : Es para moverse a un branch en especifico.
- **`git commit -am "mensaje de cambios" `**  : es para guardar cambios localmente mas no subirlos al branch.
- **`git  push origin <name branch>`**  :
- **`git checkout -b <namebranch> `**  : crea nuevo branch y te mueve automaticamente hacia el es la union de comandos 1 y 2 de esta lista.

### Comandos Para unir a la linea principal

- **`git pull request`**  : se hace normalmente en Github previo a que se revisen tus cambios en tu branch por el Review.
- **`git merge`**  : se hace tambien en Github normalmente una vez confirmado que los cambios van a la linea principal o master.
- **`git reset --merge`**  : Se Realiza para resetear algun merche hecho , y cuando ya tienes dms código debes de elgir como solucionar el conflicto si eliminando el archvio de tu rama master o de alguna otra rama.

### Comandos de seguimiento 

- **`git reset --hard`**  : Me va a resetear al ultimo `commit` que tengo, es en el caso que no quiera los cambios que he hecho .
- **`git log `**  : Es un historial de lo que ha sucedido en el tiempo (con la letra `q` sales del comando ), si le agregas `--oneline` te sale en una sola linea el historial y si le agregas `--graph` te presentara los cambios de una manera mas visual de tus cambios.
- 

### Comandos de Alias de acceso rapido
- **`git log `**  : este comando es solo el generico para ser mas especifico utilizare un comando mas detallado que es super util.
  `git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"`

- **`git status --short`**  : agregando como alias a este comando para no escribir tanto codigo en git.
  `git config --global alias.s status --short`
  
