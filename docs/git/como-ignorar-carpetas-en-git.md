### Esto es para ignorar carpetas y archivos que habian sido commiteados a git y github que no deberia serlo, y que sepas como quitarlos de git y comenzarlos a ignorarlos en .gitignore

1. Corre este comando en la carpeta raíz para remover de git esa carpeta que esté en todos lados en tu proyecto:

        git rm -r -cached nombreDeTuCarpetaOArchivo

2. Luego, agrega **`nombreDeTuCarpeta`** **de nuevo**  a .gitignore aun si ya lo tenías, para que lo comience a ignorar otra vez, esto es necesario para que funcione