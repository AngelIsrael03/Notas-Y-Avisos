# 📝 Tablero de Avisos y Notas

Aplicación desarrollada en **Go** con interfaz web en HTML y CSS, que permite agregar, editar y eliminar notas y avisos.

---

## 🧠 Descripción general

Este proyecto forma parte del curso _Tópicos para el Despliegue de Aplicaciones_. Tiene como propósito desarrollar una aplicación cliente-servidor funcional, contenedorizada y versionada correctamente.

---

## 🚀 Cómo ejecutar el proyecto en un contenedor Docker (Linux)

> Asegúrate de tener Docker Desktop instalado.

### 🔧 1. Construir la imagen Docker

Abre la terminal en la carpeta del proyecto y ejecuta:

```bash
docker build -t notas-y-avisos .
```

### ▶️ 2. Ejecutar el contenedor
```bash
docker run -d -p 8080:8080 --name tablero -v ${PWD}/notas-y-avisos.db:/app/notas-y-avisos.db notas-y-avisos
```

### 🌐 3. Abrir en el navegador

http://localhost:8080

---