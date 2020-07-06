.. Renegados documentation master file, created by
   sphinx-quickstart on Tue Aug 26 14:19:49 2014.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Introducción a Github
=====================

Pre-requisitos
##############

Instalando Visual Studio
************************
Descarga la version para cualquier sistema desde este Link `Visual Studio Code <https://code.visualstudio.com>`_

Instalar Git
############

Todo sistema
************

Descarga la version para cualquier sistema desde este Link `GIT <https://git-scm.com/downloads>`_

* Para MAC con brew

.. code-block:: 
   
   brew install git


¿Qué es GitHub?
###############

Creando nuestro primer repositorio
**********************************

1. Crear un repositorio nuevo en GitHub llamado **github-intro-XXX** (XXX serán las iniciales de tu primer nombre y tus dos apellidos). Para evitar errores, no inicialices el nuevo repositorio con archivos README licencia o gitingnore. Puedes agregar estos archivos después de que tu proyecto se haya subido a GitHub.

   .. image:: ../images/repo-create.png

|

2. Ejecuta el siguiente comando en tu terminal (XXX serán las iniciales de tu primer nombre y tus dos apellidos)
    
   .. code-block:: shell
      
      mkdir github-intro-XXX

|

3. Cambiar al directorio de trabajo que acabas de crear.

   .. code-block::  shell
      
      cd github-intro-XXX

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



