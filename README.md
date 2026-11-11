
# Proyecto DevOps - Reserva de Horas Médicas

## 1. Descripción del proyecto

Este proyecto corresponde a una aplicación web estática
que simula un sistema de reserva de horas médicas para
el Centro Médico Salud Integral.

Fue desarrollado como parte de la evaluación de DevOps
de IACC, aplicando conceptos de contenedores,
control de versiones y automatización de entornos.

La aplicación utiliza HTML, CSS, Nginx y Docker.

## 2. Objetivo

Implementar un entorno local reproducible utilizando
Docker Desktop y Docker Compose, evitando diferencias
de configuración entre equipos de desarrollo y pruebas.

## 3. Tecnologías utilizadas

- HTML5
- CSS3
- Nginx Alpine
- Docker Desktop
- Docker Compose
- Git
- GitHub
- Visual Studio Code

## 4. Estructura del proyecto

proyecto-devops-reservas-medicas/
- src/
  - index.html
  - styles.css
- Dockerfile
- docker-compose.yml
- .env.example
- .gitignore
- README.md

## 5. Requisitos previos

Para ejecutar el proyecto es necesario contar con:

- Docker Desktop instalado.
- Docker Engine en funcionamiento.
- Docker Compose disponible.
- Navegador web.

## 6. Construcción de la imagen

Desde la carpeta principal del proyecto ejecutar:

```powershell
docker compose build
```

## 7. Iniciar el servicio

Ejecutar:

```powershell
docker compose up -d
```

## 8. Acceder a la aplicación

Abrir el navegador e ingresar a:

http://localhost:8080

## 9. Verificar el contenedor

```powershell
docker compose ps
```

## 10. Consultar registros

```powershell
docker logs reservas-medicas
```

## 11. Monitorear recursos

```powershell
docker stats --no-stream
```

## 12. Detener el servicio

```powershell
docker compose down
```

## 13. Seguridad

- No se utilizan credenciales reales.
- No se almacenan datos personales.
- Se utiliza .gitignore para excluir archivos privados.
- El archivo .env.example contiene valores de ejemplo.
- La aplicación no utiliza base de datos ni API.

## 14. Limitaciones

La aplicación es una simulación académica.

El formulario no realiza reservas reales ni
almacena información de pacientes.

## 15. Autor

Proyecto desarrollado para la asignatura DevOps
de IACC, año 2026.
