# Usa la imagen base de NGINX
FROM tiangolo/nginx-rtmp

# Instala modulo RMTP
RUN mkdir -p /etc/nginx/temp/hls/

# Copia la configuración de NGINX y los certificados al contenedor
COPY ./nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./nginx/certs /etc/nginx/certs
