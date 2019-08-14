# Gestão Empresarial

Arquitetar e implementar uma solução fullstack.

## API - Backend

* /api/registry     POST        Registra um novo usuário.
* /api/user/<:id>   POST        UPDATE
* /api/users        GET         Busca todos os usuários.
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

## Database MySQL

CREATE TABLE usuarios IF NOT EXISTS (
    id_usuario
);