# git clone

El comando `git clone` permite clonar un repositorio remoto a tu máquina local. Es el primer paso para empezar a trabajar con un repositorio existente.

## Uso Básico

```bash
git clone <URL-del-repositorio>
```

Ejemplo:

```bash
git clone https://github.com/usuario/repositorio.git
```

## Ejercicio

1. Crea una carpeta en tu computadora.
2. Usa **git clone** para clonar este repositorio en esa carpeta.
3. Verifica que los archivos se hayan descargado correctamente.

## Solución al Ejercicio: `git clone`

Este ejercicio te guiará para clonar un repositorio remoto en tu máquina local y verificar que los archivos se hayan descargado correctamente.

### Pasos

1. **Crea una carpeta en tu computadora**

    Abre una terminal o línea de comandos y navega a la ubicación donde deseas crear la nueva carpeta. Luego, crea la carpeta ejecutando:

   ```bash
   mkdir mi_carpeta
   ```

2. **Navega a la carpeta**
  
    Cambia al directorio de trabajo dentro de la carpeta recién creada:

   ```bash
   cd mi_carpeta
   ```

3. **Clona el repositorio en esta carpeta**
  
    Usa el comando git clone seguido de la URL del repositorio que deseas clonar. Por ejemplo, para clonar el repositorio https://github.com/usuario/repositorio.git, ejecuta:

   ```bash
    git clone https://github.com/usuario/repositorio.git
   ```

    Esto creará una subcarpeta dentro de mi_carpeta con el nombre del repositorio (en este caso, repositorio) y descargará todos los archivos en ella.

4. **Verifica que los archivos se hayan descargado correctamente**
    
    Navega a la carpeta del repositorio recién clonado:
    
     ```bash
     cd repositorio
     ```
