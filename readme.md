# RESTFUL simples utilizando Laravel com Passport

Versão do laravel 5.6 | php >= 7.2

Detalhes da instalação

* Rodar comando `composer update`
* Instalar banco de dados e tabela
* Comando opcional: `php artisan serve` para server interno do laravel ou
* Localhost utilizando seu servidor predileto
* Ferramenta recomendada para testes `Postman`

Exemplo cadastro de teste utilizando o postman:

````json
[
    {
        "key":"name",
        "value":"AppWeb",
        "description":"",
        "type":"text",
        "enabled":true
    },
    {
        "key":"email",
        "value":"app@web.com",
        "description":"",
        "type":"text",
        "enabled":true
    },
    {
        "key":"password",
        "value":"123456",
        "description":"",
        "type":"text",
        "enabled":true
    },
    {
        "key":"c_password",
        "value":"123456",
        "description":"",
        "type":"text",
        "enabled":true
    }
]
````

Login de teste utilizando postman:

````json
[
    {
        "key": "username",
        "value": "app@web.com",
        "description": "",
        "type": "text",
        "enabled": true
    },
    {
        "key": "password",
        "value": "123456",
        "description": "",
        "type": "text",
        "enabled": true
    },
    {
        "key": "grant_type",
        "value": "password",
        "description": "",
        "type": "text",
        "enabled": true
    },
    {
        "key": "client_id",
        "value": "2",
        "description": "",
        "type": "text",
        "enabled": true
    },
    {
        "key": "client_secret",
        "value": "4KQgL5H5fq4x9zoTaLUuetgpxX8pty8HoLdDs2TL",
        "description": "",
        "type": "text",
        "enabled": true
    }
]
````

Fonte do treinamento

````
https://itsolutionstuff.com/post/php-laravel-56-rest-api-with-passport-tutorialexample.html
````

Url disponíveis

````html
Login: Verb:GET, URL:http://localhost:8080/restful/public/oauth/token
Register: Verb:GET, URL:http://localhost:8080/restful/public/api/register
List: Verb:GET, URL:http://localhost:8080/restful/public/api/products
Create: Verb:POST, URL:http://localhost:8080/restful/public/api/products
Show: Verb:GET, URL:http://localhost:8080/restful/public/api/products/{id}
Update: Verb:PUT, URL:http://localhost:8080/restful/public/api/products/{id}
Delete: Verb:DELETE, URL:http://localhost:8080/restful/public/api/products/{id}
````