# Jogo do Pac-Man

Este projeto é uma implementação do clássico **Pac-Man** em **Node.js + React**, rodando em arquitetura **Client/Server**.

---

## Estrutura do Projeto

* **/server** → Contém o servidor Node.js responsável pela lógica de jogo e comunicação.
* **/acervo-digital-hub** → Frontend em **React/Next.js**, onde o usuário interage com o jogo.

---

## Instalação

Clone o repositório:

```bash
git clone https://github.com/Jackson90989/Jogo-do-Pacman.git
cd Jogo-do-Pacman
```

### 🔹 Backend (Servidor)

```bash
cd server
npm install
node server.js
```

O servidor iniciará na porta configurada (por padrão `http://localhost:3001`).

### 🔹 Frontend (Cliente)

```bash
cd acervo-digital-hub
npm install
npm run dev
```

---

## 🎮 Como Jogar

* Use as **setas do teclado** para mover o Pac-Man.
* O objetivo é **comer todas as bolinhas** e evitar os fantasmas.
* Pontuação é atualizada em tempo real.

---

## 🐞 Bugs Conhecidos

* **Interface de vidas não atualiza corretamente**

  * Arquivo: `acervo-digital-hub/src/pages/Desafio.tsx`
  * Problema: O contador de vidas não reflete a perda ou ganho em tempo real.

* **Sincronização de vidas no servidor**

  * Arquivo: `server/server.js`
  * Problema: O backend não está enviando corretamente os eventos de atualização de vida para o cliente.
