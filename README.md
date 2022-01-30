# Simples crud de livros SPA

Aplicação é dividade em duas partes

A primeira é uma api rest com laravel 5.8, a segunda é um spa com angular 8; 

Foi usado:
 
 - php 7
 - mysql 8
 - angular cli 8
 - node 10


É necessario configurar uma base de dados mysql que será usada para o laravel. Dentro pasta da api editar as configuração de conexão no
arquivo .env de acordo com seu ambiente

    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=library-manager
    DB_USERNAME=root
    DB_PASSWORD=

Dentro desta mesma pasta executar no terminal os seguintes comandos

    composer install
    composer dump-autoload
    php artisan config:cache
    php artisan migrate --seed
    php artisan serve
    
Dentro da pata webapp executar

    npm install
    ng serve
    
A aplicação SPA devera estar disponivel em 
    
    http://localhost:4200
    
A api rest esta rodando em 

    http://localhost:8000


