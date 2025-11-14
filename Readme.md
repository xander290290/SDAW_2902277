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