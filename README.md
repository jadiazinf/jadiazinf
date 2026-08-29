## Jesús Díaz — Full Stack Engineer

I build and operate production systems end to end, from database schema to deployed UI.
Mostly TypeScript and Go.

---

### What I build

**[La Torre](https://latorreapp.com)** — Multi-tenant SaaS for condominium administration.
Assessment engine with pro-rating by aliquot, dual currency at the official rate, FIFO
allocation of payments to charges, and bank reconciliation. Background workers handle overdue
detection, reminders and voting. Layered architecture with a typed `ok/error` result instead
of exceptions. In production with paying customers.

`TypeScript` · `Next.js 15` · `Hono on Bun` · `PostgreSQL` · `Drizzle ORM` · `Turborepo` · `pg-boss` — 2,900 automated tests

**[Artitek Payments](https://artitekpayments.com)** — Multi-tenant payment gateway integrated
with Venezuelan banking: C2P, SIMF instant debit, POS, transfers, reversals and hosted checkout.
Per-tenant isolation, idempotency by external reference, signed webhooks with retries, a circuit
breaker over the bank, consumer identity via mTLS, and card data redacted at the type level
(OWASP ASVS Level 2).

`Go` · `Fiber` · `PostgreSQL` · `mTLS` — 30 domains in a hexagonal architecture, 740 automated tests

**Artitek Extraction** — LLM document extraction microservice. Async API with signed webhooks
that returns typed data with per-field confidence, never a verdict. An evaluation harness against
a hand-labelled golden set compares models on accuracy and cost per document, and the confidence
threshold routes to human review before an amount ever reaches a ledger.

`Go` · `PostgreSQL` · model evaluation against a golden set

> Most of my work lives in private repositories under [@artitek](https://github.com/artitek),
> so this profile shows less than the contribution graph does.

---

### Stack

**Languages** TypeScript · JavaScript · Go · SQL
**Frontend** React · Next.js · Tailwind CSS · React Query
**Backend** Node.js · Bun · Hono · Fiber · Ruby on Rails · REST · tRPC · microservices
**Data** PostgreSQL · Drizzle ORM · schema design and migrations
**Infra** Docker · CI/CD · GitHub Actions · mTLS · OAuth
**Practices** TDD · unit and integration testing · hexagonal architecture · monorepos

---

### Elsewhere

[jadiazinf.com](https://jadiazinf.com) · [linkedin.com/in/jadiazinf](https://www.linkedin.com/in/jadiazinf) · [artitek.dev](https://artitek.dev) · jadiaz.inf@gmail.com
