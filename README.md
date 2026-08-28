# Mohammad Reza Fatolahi

Backend engineer on the futures market-making desk at **Tabdeal**, a crypto exchange.
I own the four services behind the platform — zero to ~50 markets, millions of orders a
day against multi-million-dollar balances, 99.9% uptime. When a bug is a direct financial
loss, correctness under concurrency stops being an academic interest.

CS at Sharif, now an MBA in Strategy alongside the job.

📄 **[mrfatolahi1.github.io](https://mrfatolahi1.github.io)** · fatol.work@gmail.com

---

### Selected work

**[Yadakchi](https://github.com/mrfatolahi1/Yadakchi)** — a vertical price-comparison
engine for automotive spare parts, answering the two questions generic comparison sites
can't: does this part fit your car, and is it genuine, OEM, aftermarket, used, or
refurbished. Ten fully independent services communicating only through Kafka events
carrying full payloads, so any service can replay history and rebuild its own state.
Isolation is enforced rather than trusted — all 56 forbidden cross-service database
connections are proven refused by an automated check.
`Django 5 · Django Ninja · Kafka · PostgreSQL · Redis · Typesense · MinIO · Prometheus`

**[Crypto-Matching-Engine](https://github.com/mrfatolahi1/Crypto-Matching-Engine)** —
deterministic price–time priority matching. Runs single-threaded to rule out race
conditions and double spending, holds the live book in Redis, and guarantees exact crash
recovery by replaying a PostgreSQL event log over periodic snapshots. Ships concurrency
tests, recovery tests, Locust load tests, and OpenAPI docs.
`Python · DRF · Redis · Celery · PostgreSQL · Docker Compose`

**[Jasem](https://github.com/mrfatolahi1/Jasem)** — plain-text task, time, and expense
tracker for the terminal. On PyPI, used daily. Natural-language capture through a
pluggable LLM layer (local Ollama, OpenAI-compatible, or Anthropic) that degrades
gracefully to regex when no model is reachable. Zero runtime dependencies, Markdown
storage, Jalali calendar support, MIT.
`pipx install jasem`

**[dericer-core](https://github.com/mrfatolahi1/dericer-core)** — local-first personal
finance core library on npm. Hexagonal architecture: pure domain layer, use-case services,
storage and time behind ports, so one engine can back a desktop, web, or mobile app.
`TypeScript`

Also here: **[go-auth](https://github.com/mrfatolahi1/go-auth)** (JWT auth service in Go),
**[Lambda_Server](https://github.com/mrfatolahi1/Lambda_Server)** (Spark/Kafka/Cassandra
lambda-architecture pipeline in Scala), and
**[zare_bin](https://github.com/mrfatolahi1/zare_bin)** (event-driven URL shortener,
Spring Boot + Kafka).

---

### Toolbox

**Languages** Python, Java · *familiar:* Go, Scala, TypeScript
**Backend** Django, DRF, Spring Boot, Celery, Kafka, WebSockets, microservices
**Data** PostgreSQL, MySQL, Oracle, Redis, Elasticsearch
**Infra** Docker, Linux, CI, Grafana, on-call>
