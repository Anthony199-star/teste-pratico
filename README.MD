# Teste Prático

Este projeto é uma aplicação web desenvolvida em **Node.js** com **Express**, conectada a um banco de dados MySQL. O objetivo é implementar um sistema simples de **cadastro**, **edição**, **remoção** e **listagem** de usuários.

---

## 🛠 Tecnologias Utilizadas

- **Node.js**: Ambiente de execução JavaScript para o back-end.
- **Express**: Framework para criação de servidores e gerenciamento de rotas.
- **MySQL**: Sistema de banco de dados relacional.
- **Handlebars**: Mecanismo de template para renderização dinâmica de páginas HTML.
- **Bootstrap**: Framework para estilização e responsividade.
- **Nodemon**: Ferramenta para desenvolvimento, que reinicia automaticamente o servidor após alterações.

---

## 📂 Estrutura do Projeto

- **`app.js`**: Arquivo principal que configura o servidor Express, define as rotas e gerencia a conexão com o banco de dados MySQL.
- **`views/`**: Contém os arquivos Handlebars responsáveis por renderizar as páginas HTML do projeto.
- **`css/`**: Diretório para estilos personalizados em CSS.
- **`node_modules/`**: Diretório gerado pelo npm, onde estão as dependências instaladas.
- **`package.json`**: Arquivo de configuração do projeto Node.js, listando dependências e scripts.

---

## 🚀 Configuração e Instalação

### **Pré-requisitos**
Certifique-se de ter instalado em sua máquina:
- **Node.js** (v16 ou superior)
- **MySQL**
- **npm** (Node Package Manager)

### **Passos para configurar o projeto**

Entre no diretório do projeto

bash
cd teste-pratico
Instale as dependências do projeto

bash
npm install
Configure o Banco de Dados:

Abra o MySQL e crie o banco de dados com o nome teste_pratico.

Crie a tabela necessária para o sistema:

sql
CREATE TABLE cadastro (
    id_usuario INT AUTO_INCREMENT PRIMARY KEY,
    Nome VARCHAR(255),
    Email VARCHAR(255),
    Data_nacimento DATE
);
Inicie o Servidor

Para iniciar o servidor com reinicialização automática, use o Nodemon:

bash
npx nodemon app.js
O servidor será iniciado em http://localhost:8080.

🧑‍💻 Utilização
Rotas Principais
/: Página principal, exibe o formulário de cadastro de usuários.

/ListaUsuarios: Lista todos os usuários cadastrados no banco de dados.

/editar/:id_usuario: Exibe o formulário para edição de um usuário com base no ID.

/remover/:id_usuario: Remove o usuário do banco de dados com base no ID.

Funcionalidades
Cadastro de Usuários

Preencha os campos no formulário da página inicial e clique no botão "Cadastrar".

O usuário será salvo no banco de dados e listado na página de usuários.

Edição de Usuários

Na lista de usuários, clique no botão "Editar" correspondente.

Atualize as informações no formulário e clique em "Salvar".

Remoção de Usuários

Na lista de usuários, clique no botão "Remover" para excluir um registro.

📋 Dependências Instaladas
As principais dependências do projeto estão listadas no arquivo package.json:

Express: Framework web para gerenciamento de rotas.

Express-Fileupload: Suporte para upload de arquivos.

Express-Handlebars: Renderização dinâmica de páginas.

MySQL2: Driver para conexão com o banco de dados.

Bootstrap: Estilização responsiva com classes pré-definidas.

Nodemon: Atualização automática do servidor durante o desenvolvimento.

Para instalar todas as dependências, basta rodar:

bash
npm install
✨ Autor
Anthony Heder Rodrigues Calixto Contato e redes sociais:

LinkedIn: Seu LinkedIn

GitHub: Seu GitHub
