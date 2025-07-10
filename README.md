# NLW Agent LetMeAsk API

API desenvolvida durante a **NLW Agents** da Rocketseat, utilizando tecnologias modernas para criar uma aplicação robusta e escalável.

## 🚀 Tecnologias

- **Fastify** - Framework web rápido e eficiente
- **Drizzle ORM** - ORM type-safe para PostgreSQL
- **PostgreSQL** - Banco de dados relacional
- **TypeScript** - Linguagem de programação tipada
- **Zod** - Validação de schemas
- **Biome** - Linter e formatter
- **Docker** - Containerização

## 📋 Pré-requisitos

- Node.js 18+
- Docker e Docker Compose
- PostgreSQL (via Docker)

## ⚙️ Configuração

1. **Clone o repositório**

```bash
git clone <repository-url>
cd nlw-agent-letmeask-api
```

2. **Instale as dependências**

```bash
npm install
```

3. **Configure as variáveis de ambiente**

```bash
cp .env.example .env
# Edite o arquivo .env com suas configurações
```

4. **Inicie o banco de dados**

```bash
docker-compose up -d
```

5. **Execute as migrações**

```bash
npm run db:migrate
```

6. **Execute o seed (opcional)**

```bash
npm run db:seed
```

## 🏃‍♂️ Executando o projeto

**Desenvolvimento:**

```bash
npm run dev
```

**Produção:**

```bash
npm start
```

## 📊 Estrutura do Projeto

```
src/
├── db/
│   ├── connection.ts    # Conexão com banco
│   ├── migrations/      # Migrações do Drizzle
│   ├── schema/          # Schemas do banco
│   └── seed.ts         # Dados iniciais
├── http/
│   └── routes/         # Rotas da API
├── env.ts              # Configurações de ambiente
└── server.ts           # Servidor Fastify
```

## 🛠️ Scripts Disponíveis

- `npm run dev` - Executa em modo desenvolvimento com hot reload
- `npm start` - Executa em modo produção
- `npm run db:generate` - Gera novas migrações
- `npm run db:migrate` - Executa migrações pendentes
- `npm run db:seed` - Popula o banco com dados iniciais

## 📝 Padrões de Projeto

- **Clean Architecture** - Separação clara entre camadas
- **Type Safety** - TypeScript em todo o projeto
- **Schema Validation** - Zod para validação de dados
- **Database Migrations** - Controle de versão do banco
- **Environment Configuration** - Configurações centralizadas

## 🔧 Desenvolvimento

Este projeto foi desenvolvido durante a **NLW Agents** da Rocketseat, focando em boas práticas de desenvolvimento e arquitetura limpa.

---

Desenvolvido com ❤️ durante a NLW Agents
