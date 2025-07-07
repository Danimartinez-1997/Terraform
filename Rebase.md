Limpieza del historial de commits con git rebase interactivo

Pasos realizados:

    Hice varios commits con mensajes poco claros, como:

        cambios

        update

        cosas

    Ejecuté el comando para editar los últimos 5 commits:
    git rebase -i HEAD~5

    En el editor que se abrió, realicé lo siguiente:

        Cambié "pick" por "reword" para editar mensajes y hacerlos más descriptivos.

        Usé "squash" para fusionar commits relacionados.

        Reorganicé commits para que tuvieran un orden lógico.

    Guardé los cambios, completé los pasos del rebase y resolví cualquier conflicto si apareció.

    Finalmente, forcé el push al repositorio remoto:
    git push --force origin main

Precauciones:

    Me aseguré de que nadie más trabajara en la rama antes de forzar el push.

    Revisé cuidadosamente el nuevo historial de commits antes de subirlo.

    Añadí un archivo .gitignore para evitar subir archivos innecesarios o pesados.
