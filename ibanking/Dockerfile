# Usar una imagen base de Python
FROM python:3.9

# Crear y establecer el directorio de trabajo
WORKDIR /app

# Copiar archivos de requerimientos
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Copiar el resto de la aplicación
COPY . .

# Exponer el puerto
EXPOSE 5000

# Comando para ejecutar la aplicación
CMD ["python", "app.py"]
