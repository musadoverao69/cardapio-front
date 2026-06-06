# 🍽️ Cardápio — Frontend

Interface web de um cardápio de comidas, desenvolvida em **React + TypeScript + Vite**. Consome a API de Comidas (backend em Spring Boot) e exibe os pratos do cardápio com nome, foto e preço.

Projeto de estudo desenvolvido com base no vídeo da **Fernanda Kipper**:
👉 https://youtu.be/lUVureR5GqI

> 💡 Este é o **frontend** do projeto. Ele depende da API (backend em Java/Spring Boot), que fica em um repositório separado e precisa estar rodando para o cardápio carregar.

---

## 🛠️ Tecnologias

- **React 19**
- **TypeScript**
- **Vite** — bundler e servidor de desenvolvimento
- **ESLint** — padronização de código

---

## 🚀 Como rodar

### Pré-requisitos

- Node.js
- Backend da API rodando em `http://localhost:8080`

### Passos

```bash
# instalar dependências
npm install

# rodar em modo de desenvolvimento
npm run dev
```

A aplicação sobe em `http://localhost:5173` (porta padrão do Vite).

### Outros scripts

```bash
npm run build     # build de produção
npm run preview   # pré-visualizar o build
npm run lint      # rodar o ESLint
```

---

## 🔗 Integração com a API

O frontend consome o endpoint `GET /food` do backend, que retorna a lista de itens do cardápio:

```json
[
  {
    "id": 1,
    "title": "Rabanada Dourada",
    "image": "https://www.themealdb.com/images/media/meals/927vvp1779732018.jpg",
    "price": 24
  }
]
```

Certifique-se de que o backend esteja rodando antes de iniciar o frontend.

---

## 🙏 Créditos

Projeto desenvolvido para fins de estudo, inspirado no tutorial da [Fernanda Kipper](https://youtu.be/lUVureR5GqI).
