# Práctica: Servidor Web Nginx con Docker Compose

Este proyecto implementa y despliega un servidor web **Nginx** localmente utilizando **Docker Compose**, montando un volumen persistente para servir contenido HTML estático.

## 🚀 Requisitos Previos

- [Docker Desktop](https://www.docker.com/products/docker-desktop/) instalado y en ejecución.
- Git instalado.

## 📁 Estructura del Proyecto

```text
practica-docker-nginx/
├── docker-compose.yml   # Definición del servicio Nginx y volúmenes
├── src/
│   └── index.html       # Página web estática ("Hola Mundo")
├── .gitignore
└── README.md
```

## 🛠️ Instrucciones de Uso

### 1. Iniciar el contenedor

Ejecuta el siguiente comando en la raíz del proyecto para descargar la imagen y levantar el contenedor en segundo plano:

```bash
docker compose up -d
```

### 2. Verificar el estado del contenedor

Para comprobar que el contenedor está corriendo:

```bash
docker compose ps
```

### 3. Acceder al servidor web

Abre tu navegador web y visita:

- [http://localhost](http://localhost) (o [http://127.0.0.1](http://127.0.0.1))

También puedes probarlo desde la terminal con:

```bash
curl http://localhost
```

### 4. Detener el contenedor

Cuando desees detener el servidor:

```bash
docker compose down
```

---
*Desarrollado para la práctica de DevOps / Tecnologías de Virtualización.*
