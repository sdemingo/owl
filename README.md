# OWL

(Our aWesome Links)

Sencillo agregador de enlaces para usar en servidor Unix compartido. Permite que varios usuarios compartan enlaces de HTTP como de GEMINI, los voten y los comenten. Su uso es muy sencillo. Puedes usar los siguientes comandos para trabajar:

- list:     Lista enlaces.
- view:     Muestra los detalles de un enlace (autor, fecha, comentarios, etc.).
- add:      Agrega un nuevo enlace.
- vote:     Vota un enlace. 
- open:     Abre el enlace en el navegador.
- comment:  Añade un comentario sobre un enlace
- help:     Muestra el mensaje de ayuda.


Una vez arrancado `owl` espera recibir uno de estos comandos. Cada vez que listemos los enlaces estos llevan en la parte izquierda un número que los identifica. Ese identificador será el que tengamos que usar si queremos votarlos, comentarlos, abrirlos, etc. Por ejemplo:

```
owl> list
[1] [G| 0 v| 1 c] Un enlace a través de Gemini
[2] [H| 1 v| 2 c] Enlace al github de OWL
owl> vote 2
owl> open 1
```

Toda la información que agreguemos a OWL se guarda en un fichero llamado `.owl.log` que se encuentra en nuestro directorio personal. Este fichero puede ser editado por nosotros y en caso de que queramos eliminar nuestra actividad en la aplicación bastará con borrarlo de nuestro directorio.

