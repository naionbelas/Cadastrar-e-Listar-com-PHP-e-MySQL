# README.md

## Projeto CRUD - Cadastrar Usuário

Este projeto é uma aplicação simples de CRUD (Create, Read, Update, Delete) para cadastrar usuários. Ele foi desenvolvido em PHP e utiliza o MySQL como banco de dados. O projeto pode ser executado em um servidor local utilizando o XAMPP.

### Pré-requisitos

- [XAMPP](https://www.apachefriends.org/index.html) instalado em sua máquina.
- Um navegador web para acessar a aplicação.

### Estrutura do Projeto

```
/MultipleFiles
   ├── cad_usuario.php # Página para cadastrar novos usuários
   ├── conexao.php # Arquivo de conexão com o banco de dados
   ├── edit_usuario.php # Página para editar usuários existentes
   ├── index.php # Página principal para listar usuários
   ├── proc_cad_usuario.php # Processa o cadastro de usuários
   ├── proc_edit_usuario.php # Processa a edição de usuários
   └── naion.sql # Script SQL para criar a estrutura do banco de dados

### Configuração do Banco de Dados

1. **Importar o Banco de Dados:**
   - Abra o XAMPP e inicie o Apache e o MySQL.
   - Acesse o phpMyAdmin (geralmente em `http://localhost/phpmyadmin`).
   - Crie um novo banco de dados chamado `naion`.
   - Importe o arquivo `naion.sql` para criar a tabela `usuarios`.

2. **Configurar a Conexão:**
   - No arquivo `conexao.php`, verifique se as credenciais do banco de dados estão corretas:
     ```php
     $servidor = "localhost";
     $usuario = "root"; // Usuário padrão do XAMPP
     $senha = "";       // Senha padrão do XAMPP
     $dbname = "naion"; // Nome do banco de dados
     ```

### Executando o Projeto

1. Coloque a pasta `MultipleFiles` dentro do diretório `htdocs` do XAMPP (geralmente localizado em `C:\xampp\htdocs`).
2. Abra o navegador e acesse `http://localhost/MultipleFiles/cad_usuario.php` para cadastrar um novo usuário.
3. Após o cadastro, você pode listar os usuários em `http://localhost/MultipleFiles/index.php` e editar os dados conforme necessário.

### Funcionalidades

- Cadastro de usuários com nome e e-mail.
- Edição de usuários existentes.
- Listagem de usuários cadastrados.
- Mensagens de sucesso ou erro após o cadastro e edição.

### Créditos

Este projeto foi inspirado e desenvolvido com a ajuda dos tutoriais do canal [Celkecursos](https://www.youtube.com/@celkecursos). Agradecemos pelo excelente conteúdo!

### Licença

Este projeto é de uso livre. Sinta-se à vontade para utilizá-lo e modificá-lo conforme necessário.

---

**Nota:** Este projeto é uma demonstração simples e não deve ser utilizado em produção sem as devidas medidas de segurança, como validação de entrada e proteção contra SQL Injection.
