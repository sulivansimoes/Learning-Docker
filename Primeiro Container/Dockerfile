#Imagem base
FROM node

#Local onde será colocado projeto no Docker
WORKDIR /usr/src/app

#Copia packege.json para WorkDir
COPY package.json .

#Instala pacotes do package.json
RUN npm install

#Copia todo projeto para o WorkDir
COPY . .

#Expõe imagem na porta especificada
EXPOSE 3000

# Executa index.js para rodar aplicação
CMD ["node", "index.js"]