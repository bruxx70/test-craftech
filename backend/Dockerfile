# Imagen base de Python
FROM python:3.10

# Configuración del entorno de trabajo
WORKDIR /app

# Copiar los archivos de requerimientos y la aplicación
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copiar el código del backend
COPY . .

# Exponer el puerto 8000 (Django)
EXPOSE 8000

# Comando para ejecutar el servidor de Django
CMD ["gunicorn", "-b", "0.0.0.0:8000", "core.wsgi:application"]