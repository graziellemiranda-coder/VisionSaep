# 📸 SAEPVision

### Plataforma de compartilhamento de fotografias

## 👩‍💻 Identificação

- **Aluna:** Grazielle dos Santos Miranda
- **Curso:** Técnico em Informática para Internet
- **Instituição:** SENAI

## 📌 Sobre o projeto

O **SAEPVision** é uma plataforma web desenvolvida para conectar pessoas interessadas em fotografia. O sistema permite que usuários compartilhem imagens, conheçam fotógrafos, visualizem publicações e interajam por meio de curtidas.

A proposta é oferecer um ambiente simples, intuitivo e organizado para o compartilhamento de fotografias.

## 🎯 Objetivo

Desenvolver uma aplicação web utilizando tecnologias de front-end e back-end, com integração a um banco de dados MySQL, permitindo o cadastro de usuários e o compartilhamento de fotografias.

## 🚀 Funcionalidades previstas

- Cadastro de usuários.
- Login e autenticação.
- Perfis de usuários comuns e fotógrafos.
- Publicação de fotografias.
- Visualização de imagens em uma galeria.
- Curtidas nas publicações.
- Pesquisa de usuários e fotógrafos.
- Visualização de perfis.
- Exclusão das próprias publicações.

## 🛠️ Tecnologias utilizadas

**Front-end**
- HTML5
- CSS3
- JavaScript

**Back-end**
- Node.js
- Express

**Banco de dados**
- MySQL

**Bibliotecas**
- mysql2
- bcrypt
- jsonwebtoken
- multer
- cors
- dotenv

## 📂 Estrutura de pastas

```text
VisionSaep/
│
├── README.md
│
├── database/
│   └── saepvision.sql
│
└── backend/
    ├── middleware/
    │   └── auth.js
    │
    ├── routes/
    │   ├── auth.js
    │   ├── publicacoes.js
    │   └── usuarios.js
    │
    ├── uploads/
    │
    ├── public/
    │   ├── css/
    │   │   └── style.css
    │   ├── js/
    │   │   └── app.js
    │   └── index.html
    │
    ├── database.js
    ├── server.js
    ├── package.json
    └── .env
```

## 🗄️ Banco de dados

O projeto utiliza o MySQL, com o banco de dados chamado `saepvision`.

As principais tabelas são:

| Tabela | Descrição |
|---|---|
| usuarios | Armazena os dados dos usuários cadastrados. |
| publicacoes | Armazena as informações das fotografias publicadas. |
| curtidas | Registra as curtidas realizadas nas publicações. |

O arquivo SQL para criação do banco está localizado em `database/saepvision.sql`.

## ⚙️ Como executar o projeto

### 1. Pré-requisitos

É necessário ter instalado:

- Node.js
- npm
- MySQL
- MySQL Workbench
- Visual Studio Code

### 2. Criar o banco de dados

Abra o MySQL Workbench e execute o conteúdo do arquivo:

`database/saepvision.sql`

### 3. Configurar as variáveis de ambiente

Na pasta `backend`, configure o arquivo `.env`:

```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=sua_senha
DB_NAME=saepvision
PORT=3000
JWT_SECRET=sua_chave_secreta
```

Substitua `sua_senha` pela senha utilizada no MySQL.

### 4. Instalar as dependências

Abra o terminal na pasta `backend` e execute:

```bash
npm install
```

### 5. Iniciar o servidor

Execute:

```bash
npm run dev
```

### 6. Acessar a aplicação

Abra o navegador e acesse:

```text
http://localhost:3000
```

Para verificar o status do servidor e do banco de dados:

```text
http://localhost:3000/api/status
```

## 🔐 Segurança

O projeto utiliza recursos de autenticação com JSON Web Token (JWT) e criptografia de senhas com bcrypt.

As informações de configuração e acesso ao banco de dados devem ser mantidas no arquivo `.env`, que não deve ser compartilhado publicamente.

## 📚 Considerações finais

O SAEPVision foi desenvolvido como atividade prática do curso Técnico em Informática para Internet, com o propósito de aplicar conhecimentos de programação, desenvolvimento web, integração com banco de dados e organização de projetos.

---

**SAEPVision — Compartilhando olhares, conectando pessoas.**