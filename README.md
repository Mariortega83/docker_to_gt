 # CI con Docker y GitHub Actions

Este proyecto configura integración continua (CI) para crear y publicar automáticamente una imagen Docker en Docker Hub en cada cambio del repositorio.

## Pasos

1. **Docker Hub**:  
   - Crea un token de acceso en **Account settings > Security > New Access Token**.

2. **GitHub**:  
   - Crea un repositorio con los archivos: `.github/workflows/docker-image.yml`, `.dockerignore`, `Dockerfile`, `index.html`.
   - En **Settings > Secrets**, añade:
     - `DOCKERHUB_USERNAME`: Tu usuario de Docker Hub.
     - `DOCKERHUB_TOKEN`: El token de acceso de Docker Hub.
