# git init

El comando `git init` se utiliza para inicializar un nuevo repositorio de Git en tu máquina local. Este comando crea los archivos necesarios para empezar a rastrear cambios en tu proyecto.

## Uso Básico
```bash
git init
```

## Ejercicio

En este ejercicio, pondrás en práctica los comandos básicos de Git (git init, git add, git commit, git clone, git push, entre otros) siguiendo un flujo de trabajo típico. Este ejercicio te guiará desde la creación de un repositorio local hasta la sincronización con un repositorio remoto.

1. Configura el repositorio local

    a. Crea una carpeta en tu computadora para el proyecto.
    
    b. Navega a esa carpeta y usa `git init` para inicializar un repositorio local.

2. Crea y añade un archivo

    a. Crea un archivo llamado `README.md` y escribe una breve descripción del proyecto. 

    b. Usa `git add` para añadir `README.md` al área de preparación.

3. Realiza un commit

    a. Guarda el cambio en el repositorio con `git commit`, incluyendo un mensaje descriptivo, como: `"Add initial README file"`.

4. Conecta el repositorio a un remoto y envía los cambios

    a. Si aún no tienes un repositorio remoto (por ejemplo, en GitHub), créalo y copia su URL.

    b. Conéctalo con el repositorio local usando:

    ```bash
    git remote add origin <URL-del-repositorio-remoto>
    ```

    c. Envía el commit al repositorio remoto usando `git push`.

5. Verifica los cambios

    a. Revisa el estado del repositorio y el historial de commits usando `git status` y `git log` para asegurarte de que todos los pasos se hayan realizado correctamente.

6. Edita y actualiza el archivo

    a. Abre el archivo `README.md` nuevamente y realiza algún cambio, como agregar una nueva sección.

    b. Usa `git add` y `git commit` nuevamente para guardar el cambio.

    c. Envía la actualización al repositorio remoto con `git push`.

## Solución al Ejercicio:

Este flujo te permite ver cómo se usan los comandos de Git en conjunto para gestionar cambios en un proyecto.

### Pasos

1. Inicializa el repositorio

    ```bash
    mkdir mi_proyecto
    cd mi_proyecto
    git init
    ```

2. Crea y añade un archivo

    ```bash
    echo "# Mi Proyecto" > README.md
    git add README.md
    ```

3. Realiza el commit

    ```bash
    git commit -m "Add initial README file"
    ```

4. Conecta y envía al remoto

    Si ya tienes el remoto configurado:
  
    ```bash
    git remote add origin <URL-del-repositorio-remoto>
    git push -u origin main
    ```

5. Verifica cambios y historial

    ```bash
    git status
    git log
    ```

6. Edita y actualiza

    ```bash
    echo "## Nueva Sección" >> README.md
    git add README.md
    git commit -m "Update README with new section"
    git push
    ```