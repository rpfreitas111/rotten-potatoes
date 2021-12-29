# rotten-potatoes
Objetivo deste desafio é iniciar uma aplicação à partir de um único comando.
### Requisitos da aplicação
  * Banco de dados Mongodb
    * versão 5
  * Aplicação feito em python3
    * versão 3.10.1
## Configuração importante
  * MONGODB_DB => Nome do database
  * MONGODB_HOST => Host do MongoDB
  * MONGODB_PORT => Posta de acesso ao MongoDB
  * MONGODB_USERNAME => Usuário do MongoDB
  * MONGODB_PASSWORD => Senha do MongoDB*
## Definição do projeto
  Esta aplicação irá utilizar o docker-compose para realizar todo o processo de orquestração dos container, pois a aplicação possui uma dependência de um serviço de *apoio* que é o bando de dados.
## Arquivos importantes
  * Dockerfile => arquivo responsável por gerar a imagem
  * .dockeringore  => arquivo responsável por ignorar arquivos não necessário para imagem
  * docker-compose.yml => arquivos de orquestração do **Docker-compose**
  * app.py => arquivo de definição e start da aplicação
  * .env => Aquivo que define a versão da imagem
## Comando para iniciar a aplicação
  * **docker-compose --env-file .env  up -d --build**
