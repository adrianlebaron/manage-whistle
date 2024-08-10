### Esto es para ignorar carpetas y archivos que habian sido commiteados a git y github que no deberia serlo, y que sepas como quitarlos de git y comenzarlos a ignorarlos en .gitignore

1. Corre este comando en la carpeta donde esta el archivo o carpeta que quieres remover de git:

        git rm -r --cached nombreDeTuCarpetaOArchivo

        <!-- O AGREGA */TuCarpetaOArchivo/* LOS ASTERISCOS Y DIAGONALES ALREDEDOR DEL NOMBRE DE ARCHIVO O CARPETA PARA QUE NO TENGAS QUE ENTRAR A LA CARPETA ESPECIFICA DONDE ESTA EL ARCHIVO -->

2. Luego, agrega **`nombreDeTuCarpeta`** **de nuevo**  a .gitignore aun si ya lo tenías, para que lo comience a ignorar otra vez, esto es necesario para que funcione
