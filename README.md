# SistemasDockerNginx

Para descargar la imagen de Nginx en docker:

`` docker pull nginx``.

Iniciaremos docker en el puerto 8080:

``docker run --rm -d -p 8080:80 --name web nginx `` 

# Configuración

Se buscará el archivo en este directorio /usr/share/nginx/html y lo cambiaremos por el siguiente:
/home/mateu/documentos/nginx/sites-avaliable

``docker run --rm -d -p 8080:80 --name web -v /home/mateu/documentos/nginx/sites-avaliable:/usr/share/nginx/html nginx``
![nginx](https://user-images.githubusercontent.com/91744614/168892715-22564322-3c14-4433-9560-e94a2a1a97bf.PNG)
