# Usa la imagen base de NGINX
FROM tiangolo/nginx-rtmp

# Creacion carpetas y archivos
RUN mkdir -p /etc/nginx/temp/hls/ && \
    mkdir -p /etc/nginx/html/ && \
    mkdir -p /etc/nginx/logs/ && \
    touch /etc/nginx/logs/error.log && \
    apt-get update && apt-get install nano

# Copia la configuración de NGINX y los certificados al contenedor
COPY ./nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./nginx/certs /etc/nginx/certs
