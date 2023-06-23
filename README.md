 PASOS DEL DESAFIO : 

    1. Para pausar el trabajo en una rama y para atender otro sin generar conflicto sin haber comiteado debo:

        *Usar el comando "git stash" para guardar archivos modificados .

        *si tengo archivos nuevos y archivos modificados debo usar el comando "git stash --include-untracked"
    
    2. Luego de Haber atendido la incidencia en la que se debia borrar el archivo status.js de la rama master
       vuelvo a la rama en donde me encontraba trabajando, en este caso la rama custom-navbar.

    
    3. Una vez dentro de la rama custom-navbar para renaduar el trabajo debo:

        *escribir el comando "git stash pop" para reestablecer el trabajo y las modificaciones sin commit que 
         habia realizado y posteriormente hacer el commit correspondiente, verificando con un git pull por si 
         surgieron cambios.
