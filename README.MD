# 🏎️ Formula 1 Minimal API

API leve e eficiente para aplicações web e móveis utilizando Node.js e Fastify. Este projeto consiste em uma API minimalista focada em operações básicas de consulta (CRUD simplificado), ideal para aplicações que necessitam de respostas rápidas, estrutura enxuta e fácil manutenção.

A API disponibiliza informações sobre equipes e pilotos de Fórmula 1 através de endpoints REST simples e performáticos.

---

# 🚀 Funcionalidades

- ✅ API REST minimalista
- ✅ Consulta de equipes de Fórmula 1
- ✅ Consulta de pilotos
- ✅ Busca de piloto por ID
- ✅ Estrutura simples e escalável
- ✅ Respostas em JSON
- ✅ Integração com CORS
- ✅ Fastify com alta performance

---

# 🛠️ Tecnologias Utilizadas

- Node.js
- Fastify
- TypeScript
- @fastify/cors

---

# 📂 Estrutura do Projeto

```bash
📦 formula-1-minimal-api
 ┣ 📂 src
 ┃ ┗ 📜 server.ts
 ┣ 📜 package.json
 ┣ 📜 package-lock.json
 ┣ 📜 tsconfig.json
 ┗ 📜 README.md
```

---

# 📦 Instalação

Clone o repositório:

```bash
git clone https://github.com/kaddumotta/formula-1-minimal-api.git
```

Acesse a pasta do projeto:

```bash
cd formula-1-minimal-api
```

Instale as dependências:

```bash
npm install
```

---

# ▶️ Como Executar

Execute o projeto com:

```bash
npm run dev
```

O servidor será iniciado em:

```bash
http://localhost:3333
```

---

# 📡 Endpoints da API

## 🔹 Listar Equipes

### Endpoint

```http
GET /teams
```

### Exemplo de resposta

```json
{
  "teams": [
    {
      "id": 1,
      "name": "McLaren",
      "base": "Woking, United Kingdom"
    },
    {
      "id": 2,
      "name": "Mercedes",
      "base": "Brackley, United Kingdom"
    }
  ]
}
```

---

## 🔹 Listar Pilotos

### Endpoint

```http
GET /drivers
```

### Exemplo de resposta

```json
{
  "drivers": [
    {
      "id": 1,
      "name": "Lando Norris",
      "team": "McLaren"
    }
  ]
}
```

---

## 🔹 Buscar Piloto por ID

### Endpoint

```http
GET /drivers/:id
```

### Exemplo

```http
GET /drivers/1
```

### Resposta de sucesso

```json
{
  "driver": {
    "id": 1,
    "name": "Lando Norris",
    "team": "McLaren"
  }
}
```

### Resposta de erro

```json
{
  "message": "Driver not found"
}
```

---

# ⚙️ Dependências

Instale manualmente caso necessário:

```bash
npm install fastify @fastify/cors
```

---

# 💡 Possíveis Melhorias Futuras

- Implementar CRUD completo
- Integração com banco de dados
- Sistema de autenticação JWT
- Paginação de resultados
- Filtros por equipe
- Dockerização da aplicação
- Testes automatizados
- Deploy em cloud

---

# 🎓 Projeto de Estudo

Este projeto também foi desenvolvido como parte dos estudos do curso **Formação Node.js** da DIO (Digital Innovation One), com o objetivo de praticar conceitos fundamentais de desenvolvimento backend utilizando Node.js e Fastify.

Durante o desenvolvimento foram aplicados conceitos como:

- Criação de APIs REST
- Estruturação de rotas
- Fastify
- TypeScript
- Manipulação de parâmetros
- Respostas HTTP
- Integração com CORS
- Estruturação de projetos backend

O projeto foi personalizado e expandido para fins de aprendizado, prática e evolução no desenvolvimento de APIs modernas e performáticas com Node.js.