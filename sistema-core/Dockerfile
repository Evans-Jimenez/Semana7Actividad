# Usar una imagen base de Node.js
FROM node:18

# Crear y establecer el directorio de trabajo
WORKDIR /app

# Copiar archivos del backend
COPY package.json package-lock.json ./
RUN npm install

# Copiar el resto de la aplicación
COPY . .

# Exponer el puerto
EXPOSE 8080

# Comando para ejecutar la aplicación
CMD ["node", "server.js"]
