# 🧩 Proyecto SDAW_2902277

**Autor:** Alexander  
**NRE:** ***2277  
**Asignatura:** Sistemas de Desarrollo de Aplicaciones Web  
---

## 📘 Descripción del Proyecto

El proyecto **SDAW_2902277** consiste en una pequeña aplicación web desarrollada con **Node.js** y **Express**, que muestra un mensaje de saludo personalizado en el navegador al pulsar un botón.

El objetivo de este trabajo es demostrar el uso de **Git** y **GitHub** para la gestión de versiones, trabajo con ramas, integración mediante *pull requests* y publicación de un repositorio remoto completo.

---

## 🗂️ Estructura del Proyecto

```
/SDAW_2902277
│
├─ index.html
├─ script.js
├─ package.json
├─ server.js
└─ README.md
```

---

### Descripción de los archivos

| Archivo | Descripción |
|----------|--------------|
| **index.html** | Página principal con un botón que muestra el mensaje “Hola Alexander”. |
| **script.js** | Contiene el código JavaScript que responde al evento del botón. |
| **server.js** | Configura un servidor local utilizando Express. |
| **package.json** | Archivo de configuración del proyecto Node.js. |
| **.gitignore** | Excluye la carpeta `node_modules` y otros archivos temporales. |
| **README.md** | Documentación general del proyecto. |

---

## ⚙️ Instalación y Ejecución

### 1️⃣ Requisitos previos

- [Node.js](https://nodejs.org)
- [Git](https://git-scm.com)
- [Visual Studio Code](https://code.visualstudio.com)

### 2️⃣ Pasos para levantar el servidor local

```bash
# Clonar el repositorio
git clone https://github.com/xander290290/SDAW_2902277.git

# Entrar al proyecto
cd SDAW_2902277

# Instalar dependencias
npm install express

# Iniciar el servidor
npm start
```

### ⚙️ Visualización de la página

Abre el navegador y accede a [http://localhost:3000](http://localhost:3000)

---

## 💻 Códigos de los archivos del proyecto

### 1️⃣ index.html
```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>App SDAW_XXXX</title>
</head>
<body>
  <h1>Bienvenido a mi app</h1>
  <button id="btnSaludo">Haz clic</button>
  <script src="script.js"></script>
</body>
</html>
```

### 2️⃣ script.js
```javascript
document.getElementById('saludoBtn').addEventListener('click', function() {
    alert('Hola Alexander');
});
```

### 3️⃣ server.js
```javascript
const express = require('express');
const app = express();
const PORT = 3000;

app.use(express.static(__dirname));

app.listen(PORT, () => {
  console.log(`Servidor corriendo en http://localhost:${4567}`);
});
```

### 4️⃣ package.json
```json
{
  "name": "sdaw_2902277",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "type": "commonjs",
  "dependencies": {
    "express": "^5.1.0"
  }
}
```

### 5️⃣ .gitignore
```
node_modules/
.env
.DS_Store
Thumbs.db
npm-debug.log
```

---

## 💻 Comandos Git utilizados

| Archivo | Descripción |
|----------|--------------|
| **git init** | Inicializa un nuevo repositorio local. |
| **git config user.name "Alexander"** | Configura el nombre de usuario. |
| **git config user.email "correo@"** | Configura el correo del usuario. |
| **git add .** | Añade los archivos al área de seguimiento (staging area). |
| **git commit -m "Primer commit"** | Registra los cambios en el historial. |
| **git branch -M main** | Cambia el nombre de la rama principal a "main". |
| **git remote add origin <URL>** | Conecta el repositorio local con el remoto. |
| **git push -u origin main** | Sube los cambios a Github. |

---

## 🌿 Gestión de ramas

- **rama1_alexanderayala**: Añade información técnica de los comando Git.
- **rama2_alexanderayala**: Incluye el historial de commits en una línea obtenido con git log --oneline.

---

## 📎 Enlace al repositorio remoto

🔗 https://github.com/xander290290/SDAW_2902277.git

## 🧠 Información técnica añadida desde rama 1

- git init: Inicializa un nuevo repositorio en el directorio actual.
- git add: Añade archivos o cambios al área de preparación (staging).
- git commit: Guarda los cambios añadidos al repositorio con un mensaje descriptivo.
- git branch: Crea, lista o elimina ramas.
- git merge: Fusiona el contenido de una rama con otra.
- git push: Envía los commits locales al repositorio remoto.

---

## 📜 Información técnica añadida desde rama 2

Historial del proyecto en una sola línea:

1fe073c Primer commit: Estructura base

---

## 🧠 Información técnica añadida desde rama 3
En la primera practica he aprendido los conceptos básicos de tener un repostiroio remoto

---

## 📜 Información técnica añadida desde rama 4
Para la conexión con GitLab vamos a hacer el siguiente comando:
```
git remote add origin2 https://gitlab.com/xander290290/sdaw_2277.git
```
En mi caso cambie origin por origin2 ya que ese es el nombre que le di al remoto conectado por GitHub, y seguido de esto escribi la url del repositorio en GitLab

---

## 📌 Múltiples remotos en Git

### 🔹 ¿Qué significa tener múltiples remotos?

-   Un repositorio local conectado a mas de un repositorio remoto.
-   Puedes tener la misma información en ambos remotos o diferente información en cada uno.
-   Puedes copiar las ramas que desees en un remoto y copiarlo a otra rama creada en local.

------------------------------------------------------------------------

### 🔹 Ventajas

-   🟢 Tener mayor acceso por si una plataforma no funciona.
-   🟢 Conexión entre diferentes proyectos que tengan un punto en común.
-   🟢 Poder migrar u proyecto creado en una plataforma a otra con la se esté mas cómodo.

### 🔹 Inconvenientes

-   🔴 Diferentes funciones en cada plataforma.
-   🔴 Puede crear conflictos al hacer pull con diferentes remotos.
-   🔴 Confusión al tener diferentes ramas en cada remoto o con los nombres de estos.


------------------------------------------------------------------------

### 🔹 Comandos utilizados o consultados

#### Ver los remotos configurados

``` bash
git remote -v
```

#### Agregar un remoto

``` bash
git remote add origin https://github.com/xander290290/SDAW_2902277.git
git remote add origin2 https://gitlab.com/xander290290/sdaw_2277.git
```

#### Crear ramas desde main y moverse a cada una

``` bash
git branch rama3_alexander
git branch rama4_alexander
git checkout rama3_alexander
git checkout rama4_alexander
```

#### Creación de commits

``` bash
git add . # Tambien se puede hacer solo moviendo a staging area el archivo con git add Readme.md
git commit -m "Comentario de cada rama"
```

#### Subir cambios a un remoto específico

``` bash
git push origin main
git push origin2 main
```
### Configuración del usuario 

``` bash
git push origin main
git push origin2 main
```