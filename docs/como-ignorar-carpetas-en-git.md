1. Corre este comando en la carpeta raíz para remover de git esa carpeta que esté en todos lados en tu proyecto:

        git rm --cached */nombreDeTuCarpeta/*

2. Luego, agrega `**/nombreDeTuCarpeta**` **de nuevo** si es que ya lo tenías, a .gitignore para que lo comience a ignorar