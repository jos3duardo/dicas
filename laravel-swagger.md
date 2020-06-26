#### Criando documentação com swagger
instalando pacote
```dotenv
composer require mtrajano/laravel-swagger
```

publicar provider

config/app.php
```dotenv
'providers' => [
    ...
    Mtrajano\LaravelSwagger\SwaggerServiceProvider::class,
]
```
publicar arquivo de contfiguração
```dotenv
php artisan vendor:publish --provider="Mtrajano\LaravelSwagger\SwaggerServiceProvider"
```
gerando arquvio swagger.json
```dotenv
php artisan laravel-swagger:generate > public/swagger.json

```

como utilizar o arquivo swagger  
acesse o link abaixo  [editor swagger](http://editor.swagger.io/)  

copie e cole o conteudo do arquico **swagger.json** no site
