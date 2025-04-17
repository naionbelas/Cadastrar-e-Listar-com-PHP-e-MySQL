# CRUD de Usuários em PHP

Este projeto é um sistema simples de CRUD (Create, Read, Update, Delete) para gerenciar usuários, desenvolvido em PHP. O sistema permite cadastrar, listar e editar usuários, utilizando um banco de dados MySQL.

## Pré-requisitos

- **Servidor Local**: XAMPP
- **PHP**: Versão 7.0 ou superior
- **MySQL**: Para o banco de dados

## Instalação

1. **Clone o repositório** ou faça o download dos arquivos do projeto.
   
   ```bash
   git clone <URL_DO_REPOSITORIO>
Coloque os arquivos na pasta htdocs do XAMPP. O caminho geralmente é:

Run
Copy code
C:\xampp\htdocs\seu_projeto
Crie o banco de dados:

Abra o phpMyAdmin (geralmente acessível em http://localhost/phpmyadmin).
Crie um novo banco de dados chamado naion.
Execute o script SQL necessário para criar a tabela usuarios. (O script não está incluído, mas a tabela deve ter pelo menos as colunas id, nome, email, created, e modified).
Configure a conexão:

No arquivo conexao.php, verifique se as credenciais do banco de dados estão corretas:
php
Run
Copy code
$servidor = "localhost";
$usuario = "root"; // Usuário padrão do XAMPP
$senha = ""; // Senha padrão do XAMPP
$dbname = "naion"; // Nome do banco de dados
Estrutura do Projeto
cad_usuario.php: Página para cadastrar novos usuários.
edit_usuario.php: Página para editar usuários existentes.
index.php: Página para listar todos os usuários cadastrados.
conexao.php: Arquivo responsável pela conexão com o banco de dados.
proc_cad_usuario.php: Processa o cadastro de novos usuários.
proc_edit_usuario.php: Processa a edição de usuários existentes.
Como Usar
Inicie o XAMPP e ative os módulos Apache e MySQL.
Acesse o sistema pelo navegador em http://localhost/seu_projeto/cad_usuario.php para cadastrar um novo usuário.
Após o cadastro, você pode listar os usuários em http://localhost/seu_projeto/index.php e editar os dados conforme necessário.
Créditos
Este projeto foi inspirado e desenvolvido com base nos tutoriais do canal Celke Cursos.

Licença
Este projeto é de código aberto e pode ser utilizado e modificado conforme necessário.