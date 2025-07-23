# Esse arquivo descreve como construir uma imagem

# Define a imagem base (ex: node, python, ubuntu, etc)
FROM node:latest
 
# Atualiza os pacotes do sistema para corrigir vulnerabilidades conhecidas
RUN apt-get update && apt-get upgrade -y && apt-get clean && rm -rf /var/lib/apt/lists/*

# Diretório criado /api.
WORKDIR /api

# Copiando tudo que está dentro da pasta principal 
# para o diretório criado pelo workdir.
COPY . .

# Executa a exclusão do node_modules e instala novamente as dependências.
RUN rm -rf node_modules
RUN npm i

# Comando que ira executar o projeto.
CMD ["npm", "start"]

# Porta onde o container irá rodar.
EXPOSE 5002