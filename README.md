# 🐶 Get a Pet

> Aplicação Fullstack (MERN) desenvolvida por **Daniel Andrade Santos**, com base nas aulas do **Matheus Battisti** (Udemy).

Este projeto representa meu aprendizado prático em desenvolvimento web e continuará recebendo atualizações conforme eu evoluo tecnicamente.

![Status do Projeto](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)
![License](https://img.shields.io/badge/License-MIT-blue)
![React](https://img.shields.io/badge/Frontend-ReactJS-61DAFB)
![Node](https://img.shields.io/badge/Backend-NodeJS-339933)

---

## 📖 Sobre o Projeto

O **Get a Pet** é um sistema web criado para facilitar o processo de adoção de animais.  
Ele gerencia todo o fluxo: cadastro de usuários, criação de pets, agendamento de visitas e finalização da adoção.

A ideia principal foi praticar uma aplicação completa utilizando:

- Arquitetura **MVC**
- **API RESTful** com Node + Express
- Autenticação usando **JWT**
- Upload de imagens com **Multer**
- Gerenciamento de estado no Frontend usando **Context API**
- Integração total entre Frontend e Backend

---

## 🚀 Funcionalidades

### 🔐 Autenticação e Usuários
- [x] Registro de usuários
- [x] Login com JWT
- [x] Edição de perfil com upload de imagem
- [x] Persistência de sessão

### 🐾 Gestão de Pets
- [x] Cadastro de pets com múltiplas fotos
- [x] Visualização detalhada do pet
- [x] Edição e exclusão (somente pelo dono)
- [x] Listagem completa na Home

### 🏠 Fluxo de Adoção
- [x] Agendamento de visitas
- [x] Painel “Meus Pets”
- [x] Painel “Minhas Adoções”
- [x] Conclusão de adoção (pet é removido da lista pública)

---

## 🛠️ Tecnologias Utilizadas

### **Frontend**
- React.js
- React Router
- Context API
- Axios
- React Icons
- CSS Modules

### **Backend**
- Node.js
- Express
- MongoDB + Mongoose
- JWT (JSON Web Token)
- Bcrypt
- Multer
- CORS

---

## 📦 Como Rodar o Projeto

### Pré-requisitos
- Node.js instalado  
- MongoDB rodando localmente ou via Atlas

---

### 1️⃣ Clone o repositório

```bash
git clone https://github.com/seu-usuario/get-a-pet.git
2️⃣ Inicie o Backend
bash
Copiar código
cd backend
npm install
npm start
Você deve ver no terminal:
"Conectou ao mongoose"

3️⃣ Inicie o Frontend
bash
Copiar código
cd frontend
npm install
npm start
O sistema abrirá em:
http://localhost:3000

🔗 Estrutura de Rotas da API
Usuários (/users)
Método	Rota	Descrição
POST	/register	Registra novo usuário
POST	/login	Autentica e retorna token
GET	/checkuser	Valida token
PATCH	/edit/:id	Atualiza perfil (com imagem)

Pets (/pets)
Método	Rota	Descrição
GET	/	Lista todos os pets
POST	/create	Cria novo pet (Requer token)
GET	/mypets	Pets cadastrados pelo usuário
GET	/myadoptions	Pets em que o usuário tem interesse
DELETE	/:id	Deleta pet (somente o dono)
PATCH	/schedule/:id	Agenda visita
PATCH	/conclude/:id	Finaliza adoção

📝 Autor
Daniel Andrade Santos
Projeto desenvolvido como parte do meu aprendizado e aprimorado de forma contínua ao longo do tempo.