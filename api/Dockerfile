# Use uma imagem base com Node.js
FROM node:14

# Diretório de trabalho dentro do container
WORKDIR /usr/src/app

# Copiar os arquivos de configuração da API para dentro do container
COPY package*.json ./
COPY tsconfig.json ./
COPY src ./src

# Instalar as dependências
RUN npm install

# Porta que a API irá escutar
EXPOSE 3000

# Comando para iniciar a API
CMD [ "npm", "run", "start" ]
