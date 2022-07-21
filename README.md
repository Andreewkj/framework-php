# minifrawork

This project was created on class, but modified to add return types an php 8 features. <br>
Projeto craido em aula e adicionado a tipagem com algumas adaptações utilizando o php 8.1 co docker

# Como utilizar

Para subir o docker basta entrar no dirétorio principal (miniframework), inserir o comando sudo docker-compose up -d.

Para o perfeito funcionamento do projeto precisamos utilizar o gerenciador de dependências Composer, então vá até ao container do php utilizando o comando docker-compose exec php-fpm sh e utilize o comando composer update para instalar as dependências corretamente.

Após o docker estar rodando vá até o arquivo docker-compose.yml e localize o environment do mariadb ![image](https://user-images.githubusercontent.com/62602623/180213208-3911862a-5472-488e-a0ed-ed6244e110ee.png) <br>
utilize esses dados no seu gerenciador de bando de dados para a conexão.

Após isso utilize as querys no rquivo db-refresh para criar as tabelas iniciais.

Para criar rotas no projeto, basta ir até o arquivo Route.php e adicionar um array com o mesmo padrão da url e criar uma action no arquivo IndexController.php
