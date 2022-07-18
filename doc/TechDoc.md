# • Estrategia de ramas.
La estrategia de ramas utilizada es la Mainline branch. Es simple y efectiva para equipos pequeños. Consiste en una 1 rama principal y cada desarrollador crea una rama en una funcionalidad y al terminar la actividad se hace un Merge con la rama principal a través de Pull Requests.

# • Estrategia de versionamiento semántico.
Se utiliza el Versionamiento semántico 2.0.0
El número representa el MAJOR.MINOR.PATCH, estos incrementan de acuerdo con:

1. La versión MAJOR aumenta con cambios incompatibles de la API.
2. La versión MINOR aumenta cuando se añade una nueva funcionalidad y qué compatible con la versión anterior.
3. La versión PATCH aumenta al corregir bugs que son compatibles con versiones anteriores.

# • Descripción de las etapas del pipeline.

El pipeline principal cuenta de 2 etapas principales las cuales son build y deploy.

En la etapa de build el proyecto primero se reaturan las depenencia, luego se ejecuta el build y por ultimo se ejecutan las pruebas definidas a la aplicacion. 

Luego de que la primera etapara es completada satisfactoriamente, el pipeline procede a la etapa 2 que es el deployment, en este se autentica en la herramienta de deployment para poder pushear los cambios y correr el deploy.
