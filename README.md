# Gestão Empresarial

Arquitetar e implementar uma solução fullstack.

## API - Endpoints

* /api/users        GET         Busca todos os usuários.
* /api/registry     POST        Registra um novo usuário.
* /api/user/<:id>   PUT         UPDATE
* /api/login        POST        Login do usuário.
* /api/logout       GET         Logout do usuário.            

## GIT

git config --global andre.name "Andre L S Ferreira"
git config --global andre.email andrelsf.python@gmail.com
git config --global core.editor vim
git config --global merge.tool vimdiff
git config --global color.diff auto
git config --global color.status auto
git config --global color.branch auto
git config --global color.interactive auto
git config --list

## BackEnd

### Install composer
```bash
https://getcomposer.org/
$ curl -sS https://getcomposer.org/installer -o composer-setup.php
$ HASH=a5c698ffe4b8e849a443b120cd5ba38043260d5c4023dbf93e1558871f1f07f58274fc6f4c93bcfd858c6bd0775cd8d1
$ php -r "if (hash_file('SHA384', 'composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
$ sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
```

### Starting API Usuarios

```bash
$ composer create-project laravel/lumen apiusuarios
```

routes/web.php -> app/Http/Controllers/ExampleControllers.php

### Adding Entity Usuario

mkdir app/Models
touch app/Models/Usuario.php

Adicionando o pacote Doctrine no arquivo composer.json
```
"require": {
        "php": ">=7.1.3",
        "laravel/lumen-framework": "5.8.*",
        "doctrine/orm": "^2.6.2",
        "symfony/yaml": "2.*"
    },
```

na raiz do projeto execute: `composer update`

### 

## Database MySQL

CREATE TABLE usuarios IF NOT EXISTS (
    id_usuario
);