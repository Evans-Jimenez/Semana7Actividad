# Usar una imagen base de Nginx
FROM nginx:alpine

# Copiar archivos de la aplicación
COPY . /usr/share/nginx/html

# Exponer el puerto
EXPOSE 80

# Comando para ejecutar Nginx
CMD ["nginx", "-g", "daemon off;"]
