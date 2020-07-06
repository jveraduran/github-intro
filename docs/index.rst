.. Renegados documentation master file, created by
   sphinx-quickstart on Tue Aug 26 14:19:49 2014.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Introducción a Github
=====================

Pre-requisitos
##############

**Instalando Visual Studio**

Descarga la version para cualquier sistema desde este Link `Visual Studio Code <https://code.visualstudio.com>`_

**Instalar Git**

Descarga la version para cualquier sistema desde este Link `GIT <https://git-scm.com/downloads>`_

**Para MAC con brew**

   .. code-block:: shell
      
      brew install git


¿Qué es Github?
###############

**Creando nuestro primer repositorio**

1. Crear un repositorio nuevo en Github llamado **Github-intro-XXX** (XXX serán las iniciales de tu primer nombre y tus dos apellidos). Para evitar errores, no inicialices el nuevo repositorio con archivos README licencia o gitingnore. Puedes agregar estos archivos después de que tu proyecto se haya subido a Github.

   .. image:: ../images/repo-create.png

|

2. Ejecuta el siguiente comando en tu terminal (XXX serán las iniciales de tu primer nombre y tus dos apellidos)
    
   .. code-block:: shell
      
      mkdir Github-intro-XXX

|

3. Cambiar al directorio de trabajo que acabas de crear.

   .. code-block::  shell
      
      cd Github-intro-XXX

|

4. Inicializar el directorio local como un repositorio de Git.

   .. code-block:: shell
      
      git init

|

5. Crearemos un archivo llamado **README.md** como primer archivo inicial.
   
   - Para WINDOWS
   
      .. code-block::  shell
         
         type NUL > README.md
   
   - Para MAC
   
      .. code-block::  shell
         
         touch README.md

|

6. Agregar los archivos a tu nuevo repositorio local. Esto representa la primera confirmación.

   .. code-block:: shell
      
      git add .
   
   .. note::
      Agrega el archivo en el repositorio local y lo presenta para la confirmación. Para deshacer un archivo, usa 'git reset HEAD YOUR-FILE'.

|

7. Confirmar los archivos que has preparado en tu repositorio local.

   .. code-block:: shell
      
      git commit -m "First commit"
   
   .. note::
      Commits the tracked changes and prepares them to be pushed to a remote repository. Para eliminar esta confirmación y modificar el archivo, usa 'git reset --soft HEAD~1' y confirma y agrega nuevamente el archivo.

|

8. En la parte superior de la página de Configuración rápida del repositorio de Github, haz clic para copiar la URL del repositorio remoto.

   .. image:: ../images/copy-remote-repository-url-quick-setup.png

|

9. En Terminal, agrega la URL para el repositorio remoto donde se subirá tu repositorio local.

   .. code-block:: shell
      
      git remote add origin remote repository URL
   
   .. note::
      Si deseamos verificar la nueva URL seteada, ejecutamos 'git remote -v'

|

10. Sube los cambios en tu repositorio local a Github.

   .. code-block:: shell
      
      git push -u origin master
   
   .. note::
      Pushes the changes in your local repository up to the remote repository you specified as the origin

|



