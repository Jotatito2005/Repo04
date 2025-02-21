# Ejercicio de Git y GitHub - Repositorio 04

Este es el repositorio donde realizo el ejercicio de ramas en Git.

## 4.1 - Crear el directorio `repo04` y repositorio remoto

Primero, creamos el directorio local y el repositorio tanto local como remoto:

### 1. Crear el directorio:
```bash
mkdir repo04
cd repo04
```

### 2. Inicializar el repositorio local:
```bash
git init
```

### 3. Crear el repositorio remoto en GitHub:
En GitHub, crea un nuevo repositorio llamado `repo04`.

### 4. Vincular el repositorio local con el remoto:
```bash
git remote add origin https://github.com/tu_usuario/repo04.git
```

## 4.2 - Añadir un archivo `readme.md`, hacer commit y subir cambios al remoto

### 1. Crear un archivo `readme.md` vacío:
```bash
touch readme.md
```

### 2. Añadir el archivo al repositorio:
```bash
git add readme.md
```

### 3. Hacer un commit con el mensaje correspondiente:
```bash
git commit -m "Añadir archivo readme.md vacío"
```

### 4. Subir los cambios al repositorio remoto:
```bash
git push -u origin master
```

## 4.3 - Crear una rama con tu nombre y fecha

### 1. Crear la nueva rama (usando el nombre como `joan21022025`, por ejemplo):
```bash
git checkout -b joan21022025
```

## 4.4 - Editar el archivo `readme.md`

### 1. Editar el archivo `readme.md`:
Abre el archivo `readme.md` en cualquier editor de texto y agrega el siguiente contenido:
```
Repositorio 04

Mi primer ejercicio con ramas
```

### 2. Guardar los cambios y añadir el archivo para el commit:
```bash
git add readme.md
```

## 4.5 - Hacer 3 commits desde la rama

### 1. Primer commit:
```bash
git commit -m "Editar readme.md con contenido inicial"
```

### 2. Segundo commit:
Realiza algún cambio adicional en el archivo o puedes agregar algún otro archivo. Por ejemplo, modifica un poco el contenido de `readme.md`:
```bash
echo "Esto es una prueba de commit 2" >> readme.md
git add readme.md
git commit -m "Agregar texto extra al readme.md"
```

### 3. Tercer commit:
Modifica nuevamente el archivo, agrega un nuevo contenido o realiza alguna prueba más. Por ejemplo:
```bash
echo "Última edición en readme.md" >> readme.md
git add readme.md
git commit -m "Última edición al readme.md"
```

## 4.6 - Fusionar la rama con `master` y hacer push

### 1. Fusionar la rama `joan21022025` con `master`:
Primero, cambia a la rama `master`:
```bash
git checkout master
```

Luego, fusiona la rama `joan21022025`:
```bash
git merge joan21022025
```

### 2. Subir los cambios fusionados al repositorio remoto:
```bash
git push origin master
```

## 4.7 - Eliminar la rama local

### 1. Eliminar la rama local `joan21022025`:
```bash
git branch -d joan21022025
```

## 4.8 - Visualizar el resultado

### 1. Ver el historial de los commits con un gráfico:
```bash
git log --all --oneline --decorate --graph
```

---

**Resumen**

En este ejercicio, creamos un repositorio local y remoto, realizamos una serie de cambios en un archivo `readme.md`, y luego usamos ramas para llevar a cabo tres commits. Finalmente, fusionamos la rama con `master`, subimos los cambios al repositorio remoto y eliminamos la rama local.

---

**Autor**

Joan - Fecha: 21/02/2025
