 PASOS DEL DESAFIO : 

  EJERCICIO1
  __________

    1. Para pausar el trabajo en una rama y para atender otro sin generar conflicto sin haber comiteado debo:

        *Usar el comando "git stash" para guardar archivos modificados .

        *si tengo archivos nuevos y archivos modificados debo usar el comando "git stash --include-untracked"
    
    2. Luego de Haber atendido la incidencia en la que se debia borrar el archivo status.js de la rama master
       vuelvo a la rama en donde me encontraba trabajando, en este caso la rama custom-navbar.

    
    3. Una vez dentro de la rama custom-navbar para renaduar el trabajo debo:

        *escribir el comando "git stash pop" para reestablecer el trabajo y las modificaciones sin commit que 
         habia realizado y posteriormente hacer el commit correspondiente, verificando con un git pull por si 
         surgieron cambios.


 EJERCICIO 2
 ___________

    . Para subir a produccion el proyecto en que se viene trabajando debo : 

        1. Suponiendo que existe una rama dev , me encuentro en la rama front-react realizo un pull request a la rama dev

        2. Cuando se logra mergear los cambios , luego debo crear un release y un tag porque no lo puedo subir directamente porque 
           supongo que no cuento con el acceso para hacer un merge directo lo ideal seria crear una rama release que va a 
           contener la nueva version del proyecto en caso de que no se haya creado versiones anteriores sera la primera 1.0.0.
        
        3. Verifico si hay tags creados con el comando git tag --list y agrego la nueva rama a partir de dev con el nombre de 
           la nueva version.

        4. Como no hay tags creadas va a ser la primera por lo tanto creo la rama "release/1.0.0" y me posiciono sobre ella con 
           el comando "git checkout -b release/1.0.0".

        5. Una vez dentro de la rama creo el tag con el siguiente comando : git tag -a v1.0.0 -m "1.0.0"  y luego subo esa release
           con este comando : git push origin v.1.0.0  para enviar el tag especifico a remoto.
        
        6. Por ultimo hago un pull request desde la release a master   = master <- release/1.0.0 y el merge correspondiente
