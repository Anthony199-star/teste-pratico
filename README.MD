Teste Prático – Cadastro de Usuários
Esta aplicação é uma solução para cadastro, edição, exclusão e listagem de usuários. Utiliza Node.js, Express e MySQL, juntamente com Handlebars e CSS para exibição e estilização.

Estrutura do Projeto
/teste-pratico
  ├── app.js
  ├── /views
  │     ├── cadastro.handlebars
  │     ├── ListaUsuarios.handlebars
  │     ├── EditarLista.handlebars
  │     └── layouts/main.handlebars
  ├── /css
  │     └── estilo.css
  ├── package.json
  └── README.md
- Tecnologias Utilizadas:
- Node.js: Framework de servidor JavaScript;
- Express: Framework web para Node.js;
- MySQL: Banco de dados relacional;
- Handlebars: Template engine para renderizar HTML dinâmico;
- Bootstrap: Framework CSS para estilização;
- CSS: Estilos customizados adicionais;

Configuração e Execução
1. Pré-requisitos
Certifique-se de ter instaladas as seguintes ferramentas:
Node.js
MySQL

2. Instale as Dependências
Execute o comando abaixo para instalar as dependências necessárias:

bash
npm install

3. Configure o Banco de Dados
Acesse o MySQL e crie o banco de dados:
sql
CREATE DATABASE teste_pratico;
Crie a tabela cadastro:
sql
CREATE TABLE cadastro (
    id_usuario INT AUTO_INCREMENT PRIMARY KEY,
    Nome VARCHAR(100),
    Email VARCHAR(100),
    Data_nacimento DATE
);
4. Execute a Aplicação
Inicie o servidor com o comando:

bash
node app.js
Abra o navegador e acesse: http://localhost:8080

Funcionalidades
Cadastro de Usuários

Permite adicionar usuários com Nome, E-mail e Data de Nascimento.

Listagem de Usuários

Exibe uma tabela com todos os usuários cadastrados.

Campo de pesquisa para filtrar usuários pelo nome.

Editar Usuários

Permite alterar os dados de um usuário já cadastrado.

Excluir Usuários

Remove um usuário da base de dados.

Estrutura dos Arquivos
app.js
Arquivo principal que configura o servidor, rotas e conexão com o banco de dados MySQL.

Views
Arquivos de templates Handlebars usados para renderizar as páginas HTML dinâmicas.

cadastro.handlebars: Tela de cadastro de usuários.

ListaUsuarios.handlebars: Tela de listagem de usuários com opções de edição e exclusão.

EditarLista.handlebars: Tela para editar os dados de um usuário.

CSS
Estilos personalizados no arquivo estilo.css.

Contato
Caso tenha dúvidas ou sugestões, entre em contato em: anthonyheder25@gmail.com
