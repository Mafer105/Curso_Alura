Comunicação de container realizado como no curso
criação da rede:
    * docker network create --driver bridge minha-bridge

execução do banco de dados:
    * docker run -d --network minha-bridge --name meu-mongo mongo:4.4.6

execução da aplicação:
    * docker run -d --network minha-bridge --name alurabooks -p 3000:3000 aluradocker/alura-books:1.0
