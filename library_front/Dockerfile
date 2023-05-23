# Usando uma imagem base do Node.js
FROM node:14

# Definindo o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copiando o arquivo package.json e o arquivo package-lock.json (se existir)
COPY package*.json ./

# Instalando as dependências do aplicativo
RUN npm install

# Copiando todos os arquivos do diretório atual para o diretório de trabalho
COPY . .

# Expondo a porta necessária para o aplicativo
EXPOSE 3000

# Iniciando o aplicativo
CMD ["npm", "start"]
