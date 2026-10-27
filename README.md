# ICQA-TOOL

Base de uma aplicação web para centralizar ferramentas e rotinas de ICQA.

## Tecnologias

- Next.js com App Router
- React e TypeScript
- Tailwind CSS
- PostgreSQL via `pg`
- Configuração de deploy para Railway

## Requisitos

- Node.js 24 LTS
- npm
- PostgreSQL (opcional nesta etapa)

## Execução local

```bash
npm install
```

Copie `.env.example` para `.env.local` e ajuste `DATABASE_URL` se quiser conectar um banco local. A página inicial funciona sem banco configurado.

```bash
npm run dev
```

Acesse `http://localhost:3000`.

## Verificações

```bash
npm run lint
npm run typecheck
npm run build
npm run start
```

## Estrutura

- `src/app`: páginas, layout global e rotas de API
- `src/components`: componentes compartilhados da interface
- `src/lib`: navegação e infraestrutura de banco de dados
- `railway.json`: build, start e health check para futuro deploy

Os módulos exibidos na navegação ainda não possuem regras de negócio.
