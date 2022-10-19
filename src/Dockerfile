FROM node:18.11.0
WORKDIR /app
#workdir eh criar um diretorio de trabalho
COPY package*.json ./
#as dependencias do projeto estao nos 2 package para poder instalar os pacotes
RUN npm install 
# comando para baixar as dependencias para dentro da imagem, no caso do note js eh o npm
COPY . .
#copiar tudo do projeto e colocar na imagem
EXPOSE 8080
#para expor a porta 8080, a aplicacao utiliza esta porta. No final do "server.js" tem a porta descriminada.
CMD ["node", "server.js"]
#inicializacao do node