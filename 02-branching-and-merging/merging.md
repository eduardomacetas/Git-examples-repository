# git merge

El comando `git merge` se utiliza para fusionar los cambios de una rama en otra. Este comando es útil cuando quieres unir el trabajo realizado en una rama de características o arreglo con la rama principal del proyecto.

## Uso Básico

```bash
git merge <nombre-rama>
```

Ejemplo:

Si estás en la rama `main` y deseas fusionar la rama `mi-feature` en main, usa:

```bash
git checkout main
git merge mi-feature
```

## Ejercicio

1. Crea una rama llamada `nueva-funcionalidad` y realiza un cambio (por ejemplo, crea un archivo).
2. Haz un commit en `nueva-funcionalidad`.
3. Cambia de nuevo a la rama `main` y fusiona los cambios de `nueva-funcionalidad`.

## Solución al Ejercicio

1. **Crea y cambia a la rama `nueva-funcionalidad`:**

    ```bash
    git checkout -b nueva-funcionalidad
    ```

2. **Realiza un cambio y haz un commit:**

    ```bash
    echo "Contenido de nueva funcionalidad" > nueva-funcionalidad.txt
    git add nueva-funcionalidad.txt
    git commit -m "Add nueva funcionalidad"
    ```

3. **Cambia a la rama `main` y fusiona `nueva-funcionalidad`:**

    ```bash
    git checkout main
    git merge nueva-funcionalidad
    ```