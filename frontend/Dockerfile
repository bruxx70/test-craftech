FROM node:18

# Configurar el directorio de trabajo
WORKDIR /app

# Copiar archivos de dependencias
COPY package.json package-lock.json ./

# Instalar dependencias
RUN npm install

# Copiar el código fuente
COPY . .

# Construir la aplicación
RUN npm run build

# Exponer el puerto 3000 (React)
EXPOSE 3000

# Servir la aplicación con un servidor web ligero
CMD ["npx", "serve", "-s", "build", "-l", "3000"]