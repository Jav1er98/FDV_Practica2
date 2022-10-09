## Práctica 2: Unity Perforce
## Objetivo: experimentar el control de versiones con Perforce.

1. Utilizar la herramienta HellixCore con el repositorio creado para el proyecto de la tarea 1
2. Documentar el proceso en el fichero Readme.md del proyecto creado en la tarea 
3. Modificar el fichero presentacion.txt, agregando una frase que indique tu nombre y resuma tu experiencia en el programación de videojuegos 2D y 3D.
4. Crear un fichero nuevo, tu_nombre.txt y añádelo al proyecto.
5. Crear un proyecto Unity 3D básico y agregarlo al depot de la asignatura. Tu nombre debe ser prefijo.

## Desarrollo
Para la realización de esta practica se ha realizado lo siguiente:
1. Crear una conexión al depósito FDV2223 en la ULL.
    - El primer paso es crear un Workspace, o un directorio local en nuestro PC que contendrá copias locales de ficheros almacenados en el servidor de
    Perforce y con el que deberemos sincronizarnos.Para ello, lo primero es abrir el desplegable de Workspaces y seleccionar la opción de añadir uno nuevo.
    ![Paso 1](img/17.png)
    - Esto nos abrirá una nueva ventana, en la cual deberemos especificar el nombre del Workspace, en qué directorio local lo almacenaremos y con qué 
    depots queremos sincronizarlo. En nuestro caso solo necesitamos el llamado FDV2223, por lo que eliminaremos todos los demás para que no se sincronicen 
    con nuestro Workspace. Al terminar pulsamos Ok.
    ![Paso 2](img/2.png)
    - Debemos tener cuidado al selecionar la ruta del depot, ya que contenia la ruta de /FDV2223/... en este caso la eliminamos.
    ![Paso 3](img/5.png)
    - Si el directorio que hemos especificado no existía previamente, veremos que nos lo ha creado.
    ![Paso 4](img/8.png)
    - Dentro del WorkSpace tendremos nuestro proyecto de la entrega 1 el cual subiremos al depot asignado en este caso FDV2223.
    ![Paso 5](img/9.png)
    - Pero antes de subir el proyecto se nos ha solicitado modificar el archivo presentación.txt
    ![Paso 6](img/10.png)
    - Para ello llevamos a cabo un CHECKOUT,  ya que todos los ficheros en el Workspace son de sólo lectura.la primera acción que hay que llevar a cabo es desbloquearlo para que no sea de sólo lectura y advertir al resto del equipo. Esto lo hacemos marcando con CHECKOUT. Por tanto, cuando vamos a trabajar sobre el fichero lo marcamos en P4V y automáticamente el servidor comunica al resto de clientes el estado actual del fichero.
