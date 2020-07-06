# Introducción a GitHub - A1

## Pre-requisitos

### Visual Studio Code (Opcional)

[Visual Studio Code](https://code.visualstudio.com/)

### Instalar Git


* Todo sistema

[Git](https://git-scm.com/downloads)


* Para MAC con brew

```
brew install git
```

# ¿Qué es GitHub?

# Creando nuestro primer repositorio

1. Crear un repositorio nuevo en GitHub llamado **github-intro-XXX** (XXX serán las iniciales de tu primer nombre y tus dos apellidos). Para evitar errores, no inicialices el nuevo repositorio con archivos README licencia o gitingnore. Puedes agregar estos archivos después de que tu proyecto se haya subido a GitHub.

    ![Ceate](/images/repo-create.png?raw=true)

<br />

2. Abre tu terminal

<br />

3. Ejecuta el siguiente comando (XXX serán las iniciales de tu primer nombre y tus dos apellidos)
    ```
    $ mkdir github-intro-XXX
    ```

<br />

4. Cambiar al directorio de trabajo que acabas de crear.
    ```
    $ cd github-intro-XXX
    ```

<br />

5. Inicializar el directorio local como un repositorio de Git.
    ```
    $ git init
    ```
<br />

6. Crearemos un archivo llamado **README.md** como primer archivo inicial

    * Para WINDOWS
        ```
        $ type NUL > README.md
        ```

    * Para MAC
        ```
        $ touch README.md
        ```
<br />

7. Agregar los archivos a tu nuevo repositorio local. Esto representa la primera confirmación.
    ```
    $ git add .

    # Agrega el archivo en el repositorio local y lo presenta para la confirmación. Para deshacer un archivo, usa 'git reset HEAD YOUR-FILE'.
    ```

<br />

8. Confirmar los archivos que has preparado en tu repositorio local. 
    ```
    $ git commit -m "First commit"

    # Commits the tracked changes and prepares them to be pushed to a remote repository. Para eliminar esta confirmación y modificar el archivo, usa 'git reset --soft HEAD~1' y confirma y agrega nuevamente el archivo.
    ```

<br />

9. En la parte superior de la página de Configuración rápida del repositorio de GitHub, haz clic en ![Clone-Icon](/images/clone-icon.png?raw=true) para copiar la URL del repositorio remoto.

    ![Copy-Repo](/images/copy-remote-repository-url-quick-setup.png?raw=true)

<br />

10. En Terminal, agrega la URL para el repositorio remoto donde se subirá tu repositorio local.
    ```
    $ git remote add origin remote repository URL

    # Sets the new remote

    $ git remote -v

    # Verifies the new remote URL
    ```

<br />

11. Sube los cambios en tu repositorio local a GitHub.
    ```
    $ git push -u origin master

    # Pushes the changes in your local repository up to the remote repository you specified as the origin
    ```