 <div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=210&color=0:064E3B,45:059669,100:34D399&text=FinanControl&fontSize=48&fontColor=FFFFFF&fontAlignY=38&desc=Organização%20financeira%20em%20um%20só%20lugar&descAlignY=60&animation=fadeIn" />

# 💚 FinanControl

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=500&size=18&pause=1000&color=10B981&center=true&vCenter=true&width=650&lines=Controle+financeiro+pessoal;API+REST+%7C+Web+%7C+Mobile;Tecnologia+para+organizar+suas+finanças!" />

<br>

![Projeto](https://img.shields.io/badge/Projeto-Full%20Stack-059669?style=for-the-badge)
![Ano](https://img.shields.io/badge/Ano-2026-0D9488?style=for-the-badge)
![Status](https://img.shields.io/badge/Desenvolvimento-Em%20andamento-34D399?style=for-the-badge)

</div>

---

## 💰 Sobre o projeto

O **FinanControl** é um sistema de controle financeiro desenvolvido em conjunto com o **professor Douglas Camata**, integrando conhecimentos de desenvolvimento Web, Mobile e Back-End.

O projeto possui uma arquitetura Full Stack, composta por três partes principais: uma API REST, uma aplicação Web e um aplicativo Mobile.

Seu objetivo é aplicar conhecimentos de desenvolvimento de sistemas, integração entre aplicações, gerenciamento de dados e construção de interfaces.

As aplicações compartilham a mesma API, centralizando a comunicação e o gerenciamento das informações.

## ✨ Funcionalidades e módulos

<details>
<summary><strong>🌐 Aplicação Web</strong></summary>

- Interface desenvolvida com React.
- Navegação entre telas.
- Tela de login.
- Painel principal.
- Comunicação com a API REST.

</details>

<details>
<summary><strong>📱 Aplicativo Mobile</strong></summary>

- Aplicativo desenvolvido com React Native e Expo.
- Tela de login.
- Tela principal.
- Menu lateral de navegação.
- Navegação entre telas com React Navigation.

</details>

<details>
<summary><strong>⚙️ API Back-End</strong></summary>

- API REST desenvolvida com Node.js e Express.
- Autenticação de usuários.
- Cadastro, consulta, atualização e exclusão de usuários.
- Gerenciamento de produtos e categorias.
- Integração com PostgreSQL.
- Documentação interativa com Swagger.

</details>

## 🏗️ Arquitetura do sistema

O FinanControl possui três camadas principais que trabalham em conjunto:

```mermaid
flowchart TB
    A["💻 Aplicação Web<br/>React + Vite"]
    B["📱 Aplicativo Mobile<br/>React Native + Expo"]
    C["⚙️ API REST<br/>Node.js + Express"]
    D[("🗄️ PostgreSQL")]

    A --> C
    B --> C
    C --> D
```

| Camada | Responsabilidade |
|---|---|
| 🌐 Web | Interface acessada pelo navegador |
| 📱 Mobile | Aplicativo para dispositivos móveis |
| ⚙️ API | Processamento e comunicação entre aplicações |
| 🗄️ Banco | Armazenamento das informações |

## 🛠️ Tecnologias utilizadas

### Back-End

<div align="center">

<img src="https://skillicons.dev/icons?i=nodejs,express,postgres,js" />

</div>

| Tecnologia | Utilização |
|---|---|
| Node.js | Ambiente de execução JavaScript |
| Express.js | Desenvolvimento da API REST |
| PostgreSQL | Banco de dados relacional |
| pg | Conexão com PostgreSQL |
| bcrypt | Hash de senhas |
| Swagger | Documentação da API |
| CORS | Controle de acesso entre origens |

### Front-End Web

<div align="center">

<img src="https://skillicons.dev/icons?i=react,vite,js,html,css" />

</div>

| Tecnologia | Utilização |
|---|---|
| React | Construção da interface |
| React Router DOM | Navegação entre páginas |
| Vite | Ambiente de desenvolvimento e build |
| JavaScript | Lógica da aplicação |
| ESLint | Padronização e análise do código |

### Aplicativo Mobile

<div align="center">

<img src="https://skillicons.dev/icons?i=react,js" />

</div>

| Tecnologia | Utilização |
|---|---|
| React Native | Desenvolvimento mobile |
| Expo | Plataforma de desenvolvimento |
| React Navigation | Navegação entre telas |
| Gesture Handler | Manipulação de gestos |
| Reanimated | Animações |

## 📂 Estrutura do projeto

```text
FinanControl/
│
├── api/
│   ├── app.js
│   ├── db.js
│   ├── package.json
│   ├── config/
│   │   └── swagger.js
│   └── src/
│       └── routes/
│
├── frontend/
│   └── FinanControl/
│       ├── index.html
│       ├── package.json
│       └── src/
│           ├── App.jsx
│           ├── main.jsx
│           ├── pages/
│           ├── styles/
│           └── utils.jsx
│
├── mobile/
│   └── FinanControl/
│       ├── App.js
│       ├── index.js
│       ├── app.json
│       └── src/
│           ├── pages/
│           ├── styles/
│           └── utils.js
│
└── .gitignore
```

## 🚀 Como executar o projeto

### Pré-requisitos

- Node.js
- npm
- PostgreSQL
- Expo
- Expo Go ou emulador configurado.

### 1. Clonar o repositório

```bash
git clone https://github.com/RafaelaSsilva28/FinanControl.git

cd FinanControl
```

### 2. Iniciar o Back-End

```bash
cd api
npm install
npm start
```

Configure a conexão com o PostgreSQL no arquivo `db.js`, utilizando os dados do seu ambiente local.

### 3. Iniciar o Front-End Web

Em outro terminal:

```bash
cd frontend/FinanControl
npm install
npm run dev
```

A aplicação estará disponível em:

```text
http://localhost:5173
```

### 4. Iniciar o aplicativo Mobile

Em outro terminal:

```bash
cd mobile/FinanControl
npm install
npm start
```

Para executar em uma plataforma específica:

```bash
npm run android
npm run ios
npm run web
```

## 📡 Documentação da API

A API possui documentação interativa com Swagger.

Com o servidor em execução, acesse:

```text
http://localhost:3000/swagger
```

### Principais endpoints

| Método | Rota | Descrição |
|---|---|---|
| POST | `/login` | Autenticação |
| GET | `/usuarios` | Listar usuários |
| POST | `/usuarios` | Cadastrar usuário |
| PUT | `/usuarios/:id_usuario` | Atualizar usuário |
| DELETE | `/usuarios/:id_usuario` | Excluir usuário |
| GET | `/produtos` | Listar produtos |
| POST | `/produtos` | Cadastrar produto |
| PUT | `/produtos/:id_produto` | Atualizar produto |
| DELETE | `/produtos/:id_produto` | Excluir produto |
| GET | `/categorias` | Listar categorias |
| POST | `/categorias` | Cadastrar categoria |

## 🗄️ Banco de dados

O projeto utiliza **PostgreSQL** como banco de dados relacional.

Configuração local utilizada:

| Parâmetro | Valor |
|---|---|
| Host | `localhost` |
| Porta | `5432` |
| Database | `bd_produtos` |
| Usuário | `postgres` |

> As credenciais devem ser configuradas no ambiente local e não devem ser compartilhadas publicamente no repositório.

## 📚 Conhecimentos aplicados

Durante o desenvolvimento foram trabalhados conceitos como:

- Arquitetura Full Stack.
- Desenvolvimento de APIs REST.
- Integração entre Front-End e Back-End.
- Programação com JavaScript.
- Desenvolvimento Web com React.
- Desenvolvimento Mobile com React Native.
- Banco de dados PostgreSQL.
- Operações CRUD.
- Autenticação de usuários.
- Navegação entre telas.
- Organização e estruturação de projetos.
- Documentação de APIs com Swagger.

## 👨‍🏫 Desenvolvimento e colaboração

O **FinanControl foi desenvolvido em conjunto com o professor Douglas Camata**, unindo aprendizado, orientação e aplicação prática dos conhecimentos de Desenvolvimento de Sistemas.

A colaboração contribuiu para a construção do projeto e para o aprofundamento dos conceitos de desenvolvimento Web, Mobile e Back-End.

## 🌱 Objetivo do projeto

O FinanControl representa a aplicação prática de conhecimentos adquiridos durante a formação em Desenvolvimento de Sistemas.

O desenvolvimento de três aplicações integradas permite explorar diferentes ambientes de programação e compreender como os componentes de um sistema trabalham em conjunto.

---

<div align="center">

### 💚 Organização, tecnologia e evolução!

*Transformando conhecimentos em soluções.*

<br>

<sub>Desenvolvido em conjunto com o professor Douglas Camata.</sub>

<br><br>

<img src="https://img.shields.io/badge/Desenvolvido%20com-♥%20e%20código-059669?style=for-the-badge" />

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=120&section=footer&color=0:34D399,50:059669,100:064E3B" />

</div>
