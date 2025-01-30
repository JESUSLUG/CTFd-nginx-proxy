Este repositorio alberga los archivos Docker Compose de CTFd y NGINX Proxy. Este último añade el certificado SSL proporcionado por el contenedor NGINX Proxy, modificando así el archivo Docker Compose de CTFd. Solo toma en cuenta el docker compose que hay en la raiz, los archivos de las carpetas ya no sirven :( 


Aquí tienes un README mejorado con las indicaciones:

---

# Instrucciones de Actualización

1. **Clonar el repositorio de CTFd**  
   Primero, realiza un `git clone` del repositorio de CTFd desde GitHub:

   ```bash
   git clone https://github.com/CTFd/CTFd.git
   ```

2. **Obtener el commit correcto**  
   Dirígete a la versión correspondiente del repositorio de CTFd. Asegúrate de utilizar el commit `3895558` para la actualización, que es la version actual del 29/01/2025:

   ```bash
   cd CTFd
   git checkout 3895558
   ```

3. **Actualizar el archivo `docker-compose.yml`**  
   Copia el contenido del archivo `docker-compose.yml` que se encuentra en la raíz de este repositorio (tu repositorio actual) y pégalo en el archivo `docker-compose.yml` del repositorio de CTFd que acabas de clonar. (Olvide decir que dentro de docker compose de este repo, hay un comentario # Agrega tu domnio, cambialo ... por tu ya sabes ...) 

4. **Levantar los contenedores**  
   Una vez que hayas reemplazado el archivo `docker-compose.yml`, ejecuta el siguiente comando para iniciar los contenedores en segundo plano:

   ```bash
   docker-compose up -d
   ```

Esto debería poner en marcha tu entorno de CTFd con la configuración más reciente.
