# 📚 API de Livros

Uma aplicação web desenvolvida para gerenciamento de livros, utilizando uma API REST, banco de dados MySQL e uma interface web.

## 🎯 Sobre o projeto

O projeto tem como objetivo desenvolver um sistema completo para cadastro e gerenciamento de livros.

A aplicação permite realizar as principais operações de um CRUD:

* 🟢 **Create** — cadastrar livros
* 🔵 **Read** — listar e consultar livros
* 🟠 **Update** — atualizar informações
* 🔴 **Delete** — excluir livros

Cada livro possui as seguintes informações:

| Campo            | Descrição                         |
| ---------------- | --------------------------------- |
| `id`             | Identificador único do livro      |
| `titulo`         | Título do livro                   |
| `autor`          | Autor do livro                    |
| `ano_publicacao` | Ano de publicação                 |
| `disponivel`     | Indica se o livro está disponível |

---

## 🛠️ Tecnologias utilizadas

* 🐍 **Python**
* ⚡ **FastAPI**
* 🚀 **Uvicorn**
* 🗄️ **MySQL**
* 🔌 **SQLAlchemy**
* 🐬 **PyMySQL**
* 🌐 **HTML**
* 🎨 **CSS**
* ⚙️ **JavaScript**
* 📦 **XAMPP**
* 🗃️ **phpMyAdmin**
* 💻 **Visual Studio Code**
* 🔄 **Git e GitHub**

---

## 📂 Estrutura do projeto

```text
API-LIVROS/
│
├── database/
│   └── biblioteca_db.sql
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── app/
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   └── schemas.py
│
├── .env
├── .gitignore
├── requirements.txt
└── README.md
```

---

## ⚙️ Como executar o projeto

### 1. Clone o repositório

```bash
git clone URL_DO_SEU_REPOSITORIO
```

Entre na pasta do projeto:

```bash
cd API-LIVROS
```

### 2. Crie o ambiente virtual

No Windows:

```bash
python -m venv venv
```

Ative o ambiente:

```bash
venv\Scripts\activate
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

---

## 🗄️ Configuração do banco de dados

O projeto utiliza **MySQL** para armazenar as informações dos livros.

O banco pode ser executado utilizando o **XAMPP** e administrado através do **phpMyAdmin**.

### Banco utilizado

```text
biblioteca_db
```

Para configurar:

1. Abra o XAMPP.
2. Inicie o **Apache**.
3. Inicie o **MySQL**.
4. Acesse o phpMyAdmin.
5. Crie ou importe o banco `biblioteca_db`.
6. Execute o arquivo:

```text
database/biblioteca_db.sql
```

---

## 🔐 Configuração do ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
DATABASE_URL=mysql+pymysql://root:SUA_SENHA@localhost/biblioteca_db
```

> ⚠️ O arquivo `.env` contém informações locais e não deve ser enviado para o GitHub.

---

## 🚀 Executando a API

Com o ambiente virtual ativado, execute:

```bash
uvicorn app.main:app --reload
```

A API ficará disponível localmente em:

```text
http://127.0.0.1:8000
```

A documentação automática da API pode ser acessada em:

```text
http://127.0.0.1:8000/docs
```

---

## 🔗 Principais rotas

| Método   | Rota           | Função                 |
| -------- | -------------- | ---------------------- |
| `GET`    | `/livros`      | Lista todos os livros  |
| `GET`    | `/livros/{id}` | Consulta um livro      |
| `POST`   | `/livros`      | Cadastra um novo livro |
| `PUT`    | `/livros/{id}` | Atualiza um livro      |
| `DELETE` | `/livros/{id}` | Exclui um livro        |

---

## 🌐 Front End

O sistema possui uma interface desenvolvida com **HTML, CSS e JavaScript**.

A interface permite:

* 📖 visualizar os livros cadastrados;
* ➕ adicionar novos livros;
* ✏️ editar informações;
* 🗑️ excluir livros;
* 🔎 consultar os dados da API;
* 🔄 atualizar a lista de livros.

O JavaScript utiliza `fetch()` para realizar a comunicação entre o Front End e a API.

---

## 🧪 Testes

A API pode ser testada utilizando a documentação automática do FastAPI através do Swagger.

Também podem ser realizados testes das operações:

```text
POST → Cadastrar livro
GET → Consultar livros
PUT → Atualizar livro
DELETE → Excluir livro
```

---

## 📌 Objetivos do projeto

Com este projeto, são praticados conceitos de:

* desenvolvimento de APIs REST;
* criação de rotas com FastAPI;
* operações CRUD;
* integração entre Python e MySQL;
* utilização do SQLAlchemy;
* validação de dados;
* tratamento de erros HTTP;
* desenvolvimento Front End;
* comunicação entre Front End e Back End;
* utilização do Git e GitHub.

---

## 📚 Disciplina

**Sistemas Web II — SW-II**

Projeto acadêmico desenvolvido como atividade prática da disciplina.

---

## 👨‍💻 Autor

**Victor Pacheco**

Projeto desenvolvido para fins acadêmicos e de aprendizado em desenvolvimento web.

---

## 🏁 Resultado esperado

Ao final do projeto, espera-se ter uma aplicação funcional capaz de gerenciar livros através de uma **API FastAPI**, utilizando **MySQL** como banco de dados e uma interface web desenvolvida com **HTML, CSS e JavaScript**.

O sistema deverá permitir cadastrar, visualizar, atualizar e excluir livros de maneira simples e organizada.

---

⭐ **Projeto desenvolvido para aprendizado e prática de desenvolvimento Web.**
