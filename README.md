# TechRetail - Infraestructura de Microservicios con Docker Swarm

Este proyecto implementa una arquitectura escalable y de alta disponibilidad para la plataforma de comercio electrónico **TechRetail**, resolviendo problemas de caídas del sistema y lentitud en campañas de alta demanda.

## 📋 Arquitectura del Sistema
La solución utiliza **Docker Swarm** para orquestar los siguientes microservicios:
* **Frontend:** Servidor Nginx (Escalable a 5 réplicas).
* **Backend:** Servicio REST en Node.js (2 réplicas).
* **Database:** MySQL 8.0 con persistencia de datos mediante volúmenes.
* **Cache:** Redis 7 para optimización de consultas.
* **Visualizer:** Herramienta de monitoreo gráfico del clúster.

## 🚀 Guía de Despliegue

### Requisitos previos
- Docker Desktop con Swarm activado (`docker swarm init`).
- Terminal PowerShell o Bash.

### Pasos para el despliegue
1. **Clonar el repositorio:**
   ```bash
   git clone [URL_DE_TU_REPOSITORIO]
   cd [NOMBRE_DE_TU_CARPETA]
