# git branch & git checkout -b

El comando `git branch` permite ver, crear o eliminar ramas en un repositorio. El comando `git checkout -b` crea y cambia a una nueva rama, permitiéndote trabajar en una característica o arreglo sin afectar la rama principal.

## Uso Básico

```bash
# Crear una nueva rama
git branch <nombre-rama>

# Crear y cambiar a una nueva rama
git checkout -b <nombre-rama>
```

Ejemplo:

```bash
git branch feature-nueva
git checkout -b feature-nueva
```

## Ejercicio

1. Crea una rama llamada `mi-feature`.
2. Cambia a la rama `mi-feature`.
3. Verifica en qué rama estás usando `git branch`.

## Solución al Ejercicio

1. **Crea la rama `mi-feature`:**

    ```bash
    git branch mi-feature
    ```

2. **Cambia a la rama `mi-feature`:**

    ```bash
    git checkout -b mi-feature
    ```

3. **Verifica la rama actual:**

    ```bash
    git branch
    ```
