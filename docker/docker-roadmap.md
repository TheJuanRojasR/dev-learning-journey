# Roadmap Profesional Docker para DevOps
---
# Módulo 1 — Fundamentos

## Objetivo

Entender qué es Docker internamente y qué problema resuelve.

### 1.1 Problemas previos a Docker
* "Works on my machine"
* Dependencias incompatibles
* Entornos inconsistentes
* Despliegues manuales

### 1.2 Conceptos de Sistemas Operativos necesarios

* Hardware vs Software
* Sistema Operativo
* Kernel
* Procesos
* PID
* Recursos (CPU, RAM, Disco, Red)

### 1.3 Virtualización
* Qué es una VM
* Hypervisor
* Tipos de Hypervisors
* Ventajas y desventajas

### 1.4 Contenedores
* Qué es un contenedor
* Diferencias con VM
* Beneficios
* Casos de uso

### 1.5 Tecnologías Linux detrás de Docker
* Namespaces
* Cgroups
* Union Filesystem (introducción)

### 1.6 Arquitectura Docker
* Docker Engine
* Docker Client
* Docker Daemon
* Docker Registry
* Docker Hub

### 1.7 Recursos Docker
* Imágenes
* Contenedores
* Redes
* Volúmenes

### Proyecto del módulo
* Instalar Docker
* Analizar la arquitectura de Docker en Ubuntu

### Debes ser capaz de explicar
* Qué es Docker
* Qué es una imagen
* Qué es un contenedor
* Diferencia entre VM y contenedor
* Docker Client vs Docker Daemon

---

# Módulo 2 — Comandos Esenciales

## Objetivo

Administrar contenedores utilizando la CLI.

### 2.1 Información del entorno

* `docker version`
* `docker info`

### 2.2 Gestión de imágenes

* `docker pull`
* `docker images`
* `docker image`

### 2.3 Gestión de contenedores

* `docker run`
* `docker ps`
* `docker stop`
* `docker start`
* `docker restart`

### 2.4 Diagnóstico

* `docker logs`
* `docker exec`
* `docker inspect`

### 2.5 Administración

* `docker cp`
* `docker rm`
* `docker rmi`

### 2.6 Limpieza

* `docker system prune`
* `docker system df`

### 2.7 Observabilidad básica

* `docker stats`

### Laboratorio

Levantar:

* Nginx
* Redis
* PostgreSQL

Utilizando únicamente comandos Docker.

### Debes dominar

* Crear contenedores
* Entrar a contenedores
* Ver logs
* Diagnosticar problemas básicos

---

# Módulo 3 — Docker Images

## Objetivo

Comprender qué es una imagen Docker y cómo funciona internamente.

### 3.1 Anatomía de una imagen

* Qué contiene una imagen
* Cómo se construye

### 3.2 Layers

* Qué son
* Cómo funcionan

### 3.3 Union File System

* OverlayFS
* Capas de lectura
* Capa de escritura

### 3.4 Versionado

* Tags
* latest
* Semantic Versioning

### 3.5 Distribución

* Pull
* Push
* Registries

### 3.6 Optimización

* Reducir tamaño
* Reutilizar capas

### Laboratorio

Analizar imágenes oficiales:

* Nginx
* Redis
* PostgreSQL

### Debes dominar

* Layers
* Tags
* Estrategias de versionado

---

# Módulo 4 — Dockerfile Profesional

## Objetivo

Construir imágenes listas para producción.

### 4.1 Dockerfile básico

* FROM
* RUN
* CMD

### 4.2 Configuración

* ENV
* ARG
* LABEL

### 4.3 Archivos

* COPY
* ADD

### 4.4 Ejecución

* ENTRYPOINT
* CMD
* Diferencias entre ambos

### 4.5 Organización

* WORKDIR
* USER
* EXPOSE

### 4.6 Persistencia

* VOLUME

### 4.7 Salud del contenedor

* HEALTHCHECK

### 4.8 Optimización

* Caché de construcción
* Orden de instrucciones

### 4.9 Multi-stage Builds

* Builder Stage
* Runtime Stage

### 4.10 Hardening

* Imágenes mínimas
* Usuarios no root

### Proyecto

Dockerizar una API Node.js.

### Debes dominar

* Crear Dockerfiles desde cero
* Optimizar imágenes
* Multi-stage builds

---

# Módulo 5 — Volúmenes y Persistencia

## Objetivo

Persistir información fuera del ciclo de vida del contenedor.

### 5.1 Sistemas de almacenamiento

* Capa de escritura

### 5.2 Bind Mounts

* Concepto
* Casos de uso

### 5.3 Named Volumes

* Creación
* Administración

### 5.4 Anonymous Volumes

* Funcionamiento
* Problemas comunes

### 5.5 Backups

* Exportar datos

### 5.6 Restauración

* Restaurar datos desde backups

### Proyecto

Persistir una base de datos PostgreSQL.

### Debes dominar

* Diferencias entre tipos de volúmenes
* Estrategias de backup

---

# Módulo 6 — Redes

## Objetivo

Comprender cómo se comunican los contenedores.

### 6.1 Fundamentos de Networking Docker

* Conceptos básicos

### 6.2 Bridge Network

* Funcionamiento
* Casos de uso

### 6.3 Host Network

* Ventajas
* Desventajas

### 6.4 None Network

* Aislamiento total

### 6.5 DNS Interno

* Resolución de nombres

### 6.6 Comunicación entre contenedores

* Redes compartidas

### 6.7 Publicación de puertos

* Port Mapping

### Proyecto

Conectar una API con PostgreSQL.

### Debes dominar

* Redes bridge
* DNS interno
* Publicación de puertos

---

# Módulo 7 — Docker Compose

## Objetivo

Orquestar aplicaciones multi-contenedor.

### 7.1 Introducción

* Qué es Docker Compose
* Casos de uso

### 7.2 Sintaxis YAML

* Estructura básica

### 7.3 Services

* Definición
* Configuración

### 7.4 Networks

* Redes personalizadas

### 7.5 Volumes

* Persistencia compartida

### 7.6 Environment Variables

* Variables de entorno
* Archivos `.env`

### 7.7 Depends On

* Dependencias entre servicios

### 7.8 Profiles

* Entornos personalizados

### 7.9 Override Files

* docker-compose.override.yml

### Proyecto Completo

* Frontend
* Backend
* PostgreSQL
* Redis

### Debes dominar

* Aplicaciones multi-contenedor
* Gestión de entornos

---

# Módulo 8 — Docker para Backend

## Objetivo

Aplicar Docker a tecnologías backend reales.

### Node.js

* Desarrollo
* Producción

### Java Spring Boot

* Construcción de imágenes
* Optimización

### PostgreSQL

* Configuración
* Persistencia

### MySQL

* Configuración
* Persistencia

### Redis

* Configuración
* Casos de uso

### Proyecto

API REST completa dockerizada.

---

# Módulo 9 — Seguridad

## Objetivo

Aplicar prácticas de seguridad utilizadas en producción.

### Principio de mínimo privilegio

### Usuarios no root

### Gestión de secretos

* Docker Secrets
* Variables de entorno

### Escaneo de vulnerabilidades

* Docker Scout
* Trivy

### Hardening de imágenes

### Supply Chain Security

### Debes dominar

* Construcción de imágenes seguras
* Gestión adecuada de credenciales

---

# Módulo 10 — Docker en Producción

## Objetivo

Preparar aplicaciones para entornos reales.

### Logging

### Métricas

### Monitoreo

### Observabilidad

### Escalabilidad

### Alta disponibilidad

### Estrategias de despliegue

* Rolling Update
* Blue-Green Deployment
* Canary Deployment

### Proyecto

Simulación de un entorno productivo.

---

# Módulo 11 — CI/CD

## Objetivo

Automatizar el ciclo de vida de las aplicaciones.

### GitHub Actions

### GitLab CI/CD

### Jenkins

### Pipeline Completo

1. Build
2. Test
3. Security Scan
4. Push
5. Deploy

### Proyecto

Pipeline automatizado para una aplicación dockerizada.

---

# Módulo 12 — Docker + Kubernetes

## Objetivo

Comprender la transición desde Docker hacia la orquestación.

### ¿Por qué Docker no es suficiente?

### Introducción a Kubernetes

### Pods

### Deployments

### ReplicaSets

### Services

### ConfigMaps

### Secrets

### Ingress

### Rolling Updates

### Proyecto Final

Desplegar una aplicación completa en Kubernetes.

---

# Meta Final

Al finalizar este roadmap deberías ser capaz de:

* Dockerizar aplicaciones reales.
* Crear imágenes optimizadas.
* Gestionar persistencia de datos.
* Configurar redes entre contenedores.
* Orquestar aplicaciones con Docker Compose.
* Aplicar buenas prácticas de seguridad.
* Automatizar pipelines CI/CD.
* Desplegar aplicaciones en entornos productivos.
* Comprender y utilizar Kubernetes a nivel inicial/intermedio.
