## Jesús Díaz — Full Stack Engineer

I deliver production systems in full, from data modelling to deployed interface.
Mostly TypeScript and Go.

---

### What I build

**[La Torre](https://latorreapp.com)** — Multi-tenant SaaS for condominium administration.
It manages the condominium's accounts: pro-rating of the period's expenses across units by
aliquot, multi-currency billing at the official rate, allocation of each payment to the oldest
outstanding debt, and reconciliation against the bank statement. It constitutes the
condominium's book of record, so an incorrect balance has direct consequences before the
owners' association: automated tests cover the financial flows and gate deployment, which
allows the assessment engine to be modified on buildings in operation. Residents register a
payment by photographing the receipt, and the form completes itself from the extracted data.
In production with paying customers.

`TypeScript` · `Next.js 15` · `Hono on Bun` · `PostgreSQL` · `Drizzle ORM` · `Turborepo` · `pg-boss`

**[Artitek Payments](https://artitekpayments.com)** — Multi-tenant payment gateway. It allows a
merchant to take payments in Venezuela without integrating directly with the bank: C2P, SIMF
instant debit, point of sale, transfers, reversals and hosted checkout under a single API.
Designed around the failure modes with financial impact: idempotency by external reference,
signed webhooks retried until merchant acknowledgement, and a circuit breaker that contains
bank unavailability. Scheduled reconciliation against the bank, where each movement settles
exactly one payment, which prevents the same receipt being credited twice. Per-merchant
isolation, client authentication over mTLS, and card fields redacted at the type level, which
prevents them reaching logs (OWASP ASVS Level 2).

`Go` · `Fiber` · `PostgreSQL` · hexagonal architecture · `mTLS`

**Artitek Extraction** — LLM document extraction microservice. It converts photographed
invoices and receipts into typed fields with a confidence level per field. Below the threshold,
the document is routed to human review before the amount is recorded: the service reports the
reading, it does not resolve it. Evaluated against a manually labelled set that scores each
model on accuracy and cost per document, supporting model selection with data.

`Go` · `PostgreSQL` · model evaluation against a golden set

> Most of my work lives in private repositories under [@artitek](https://github.com/artitek),
> so this profile shows less than the contribution graph does.

---

### Stack

**Languages** TypeScript · Go · SQL
**Frontend** React · Next.js · TanStack Start · Tailwind CSS · React Query
**Backend** Node.js · Bun · Hono · Fiber · Ruby on Rails · REST · tRPC
**Data** PostgreSQL · MongoDB · Drizzle ORM · schema design and migrations
**Infra** Docker · CI/CD · GitHub Actions · mTLS · OAuth
**Practices** TDD · hexagonal architecture · monorepos

---

### Elsewhere

[jadiazinf.com](https://jadiazinf.com) · [linkedin.com/in/jadiazinf](https://www.linkedin.com/in/jadiazinf) · [artitek.dev](https://artitek.dev) · jadiaz.inf@gmail.com
