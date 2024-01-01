Práctica, módulo Git y GitHub

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

    ``git reset --hard HEAD~1``

    Porque  no queremos mantener los cambios del working copy, se podría haber realizado en dos pasos con:
    ``git reset HEAD~1`` y después ``git restore <Nombre del archivo>``

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

    ``git reflog``
    ``git reset --hard <id del commit>``

    Primero busque el ID del commit que hice en el paso 10 con ``git reflog`` después lo usé para desplazarma hasta él con ``git reset --hard <id del commit>``

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

    No causó ningún conflicto, además no hizo ningún merge.
    
    Porque styled ya tiene acceso a todos los commits de main el mensaje que me da es: Already up to date.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

    Sí causó conflicto.

    Ya que la rama htmlify y la styled tienen las mismas líneas modificadas, lo resuelvo eligiendo las líneas que me interesan y realizo un nuevo commit.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

    No causó conflicto.

    Porque es un merge Fast Forward y se basa en mover la rama en la que está HEAD hasta el commit de la otra rama.

- ¿Qué comando o comandos utilizaste en el paso 25?

    ``git log --graph``
    
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

    Sí, podría ser fast forward.

    Porque la rama title tiene acceso a todos los commits de main, para que sea no fast forward lo he tenido que obligar con el comando ``git merge --no-ff <Nombre de la rama>``

- ¿Qué comando o comandos utilizaste en el paso 27?

    ``git reset HEAD~1``

- ¿Qué comando o comandos utilizaste en el paso 28?

    ``git restore <Nombre del archivo>``

- ¿Qué comando o comandos utilizaste en el paso 29?

    Lo intento con ``git branch -d <Nombre de la rama>``, pero no me deja.

    La borro con ``git branch -D <Nombre de la rama>``

- ¿Qué comando o comandos utilizaste en el paso 30?

    Busco el ID con ``git reflog`` y me muevo descartando cambios con ``git reset --hard <id del commit>``

- ¿Qué comando o comandos usaste en el paso 32?

    Busco el ID con ``git reflog`` y me muevo descartando cambios con ``git reset --hard <id del commit>``

- ¿Qué comando o comandos usaste en el punto 33?

    Busco el ID con ``git reflog`` y me muevo descartando cambios con ``git reset --hard <id del commit>``