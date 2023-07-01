# Use uma imagem base com Node.js
FROM node:18

# Diretório de trabalho dentro do container
WORKDIR /usr/src/app

# Copiar os arquivos de configuração do Nuxt.js 3 para dentro do container
COPY package*.json ./
COPY nuxt.config.ts ./
COPY .nuxt ./.nuxt

# Instalar as dependências
RUN npm init -y
RUN npm install

# Porta que o servidor do Nuxt.js 3 irá escutar
EXPOSE 3000

# Comando para iniciar o servidor do Nuxt.js 3
CMD [ "npm", "run", "dev" ]
