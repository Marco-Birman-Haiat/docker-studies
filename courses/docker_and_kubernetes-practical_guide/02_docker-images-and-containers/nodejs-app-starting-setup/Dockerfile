FROM node

WORKDIR /app

#  se a pasta não existir, será criada (/app). Se não tiver o comando WORKDIR anterior
# COPY . /app

# para facilitar a leitura, podemos explicitar que estamos copiando para /app. Mas "COPY . ." funcionaria
COPY . /app

# define comando a ser rodado durante a contrução da imagem
RUN npm install

# define a porta do container que será exposta para o OS que contem o container. Na aplicação temos app.listen(80)
# Pelo que entendi não é necessário, mas recomendado por motivos de documentação
EXPOSE 80

# define o comando chamado quando o container for iniciado!! Deve ser a última instrução
CMD [ "node", "server.js" ]
