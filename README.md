# 🎬 API Movie Flix
API RESTful para gerenciamento de filmes, construída com Node.js, TypeScript, PostgreSQL, Prisma ORM e Docker.

---

## 🚀 Visão Geral

Este projeto entrega uma API robusta para cadastro, consulta e atualização de filmes, com suporte a gêneros e idiomas. Ideal para aplicações web modernas, integrações e testes técnicos.

---

## 🛠️ Tecnologias Utilizadas

- **Node.js**
- **TypeScript**
- **Express**
- **Prisma ORM**
- **PostgreSQL**
- **Docker & Docker Compose**
- **Swagger** (documentação)
- **ESLint & Prettier** (qualidade de código)

---

## 📁 Estrutura do Projeto

```
├── src/                # Código fonte (server.ts)
├── prisma/             # Schema e migrations Prisma
├── data/               # Persistência de dados Docker
├── swagger.json        # Documentação OpenAPI
├── Dockerfile          # Container da aplicação
├── docker-compose.yml  # Orquestração dos serviços
├── package.json        # Scripts e dependências
├── tsconfig.json       # Configuração TypeScript
```

---

## ⚡ Funcionalidades

- CRUD de filmes
- Associação de gêneros e idiomas
- Validação de duplicidade de títulos
- Documentação interativa via Swagger
- Deploy containerizado (Docker)

---

## 🔗 Endpoints Principais

| Método | Rota           | Descrição                  |
|--------|----------------|----------------------------|
| GET    | /movies        | Lista todos os filmes      |
| POST   | /movies        | Cria um novo filme         |
| PUT    | /movies/:id    | Atualiza um filme          |

Para detalhes e testes, acesse: [`/docs`](http://localhost:3000/docs)

---

## 🐳 Como Executar Localmente

1. **Clone o repositório:**
	```bash
	git clone https://github.com/kalyel/API-Movie-Flix.git
	cd API-Movie-Flix
	```
2. **Suba os containers:**
	```bash
	docker-compose up --build
	```
3. **Acesse a documentação:**
	- [http://localhost:3000/docs](http://localhost:3000/docs)
4. **Banco de dados:**
	- PostgreSQL: `localhost:5432` (user: user, password: password, db: movieflix-db)
	- PgAdmin: [http://localhost:5050](http://localhost:5050) (user@email.com / password)

---

## 🧩 Prisma ORM

- Models: `Movie`, `Genre`, `Language`
- Migrations automáticas
- Configuração: `prisma/schema.prisma`

---

## 📝 Scripts Úteis

- `npm run dev` — Hot reload com TSX
- `npm run build` — Compila TypeScript
- `npm run start` — Executa versão compilada
- `npm run format` — Formata código com Prettier

---

## 🏆 Diferenciais Técnicos

- Código limpo, tipado e modular
- Validação de dados e erros claros
- Documentação OpenAPI pronta para integração
- Pronto para produção com Docker
- Padrões de mercado (ESLint, Prettier, TypeScript strict)

---

## 📚 Documentação Swagger

Acesse `/docs` para explorar e testar endpoints.

---

## 💡 Como Contribuir

1. Fork o projeto
2. Crie uma branch (`feature/nome-feature`)
3. Faça o commit
4. Abra um Pull Request