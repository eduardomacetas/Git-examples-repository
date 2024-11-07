# Resolución de Conflictos

Los conflictos de fusión ocurren cuando Git no puede fusionar automáticamente cambios en archivos porque han sido modificados de forma diferente en ambas ramas.

## Cómo Resolver Conflictos

1. Durante una fusión, Git señalará si ocurre un conflicto en un archivo.
2. Abre el archivo en conflicto; verás líneas de conflicto `<<<<<< HEAD` y `>>>>>>>`.
3. Elimina las líneas de conflicto y edita el archivo según el resultado deseado.
4. Añade el archivo modificado y haz un commit para completar la fusión.

Ejemplo de un conflicto:

```markdown
<<<<<<< HEAD
Contenido en la rama main
=======
Contenido en la rama nueva-funcionalidad
>>>>>>> nueva-funcionalidad
```

## Ejercicio

1. Crea dos ramas (`main` y `conflicto-ejemplo`).
2. Modifica el mismo archivo en ambas ramas.
3. Intenta fusionar `conflicto-ejemplo` en `main` y resuelve el conflicto que surge.

## Solución al Ejercicio: Resolución de Conflictos

1. **Crea y cambia a la rama `conflicto-ejemplo`:**

    ```bash
    git checkout -b conflicto-ejemplo
    ```

2. **Realiza un cambio en un archivo y haz un commit:**

    ```bash
    echo "Cambio en conflicto-ejemplo" > conflicto.txt
    git add conflicto.txt
    git commit -m "Cambios en conflicto-ejemplo"
    ```

3. **Cambia a la rama `main`, modifica el mismo archivo y haz otro commit:**

    ```bash
    git checkout main
    echo "Cambio en main" > conflicto.txt
    git add conflicto.txt
    git commit -m "Cambios en main"
    ```

4. **Fusiona `conflicto-ejemplo` en `main` y resuelve el conflicto:**

    ```bash
    git merge conflicto-ejemplo
    ```

5. **Añade el archivo y completa la fusión:**

    ```bash
    git add conflicto.txt
    git commit -m "Resolve conflict between main and conflicto-ejemplo"
    ```
