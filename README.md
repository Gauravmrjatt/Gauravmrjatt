# Gaurav Chaudhary

### Backend engineer — Go · Node.js · PostgreSQL · Redis · RabbitMQ

I build and run production systems: a multi-carrier logistics platform with payments, an affiliate tracking panel at 527K leads, and a self-hosted webhook delivery engine in Go.

**Numbers, not adjectives**

| | |
|---|---|
| **527K leads** from 1.77M clicks (30% conversion) | affiliate panel, INR 2.8 Cr in payments processed |
| **1,700+ orders** | multi-carrier shipping platform, ~50 franchise operators |
| **5 production systems** | all currently deployed and maintained by me |

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=Gauravmrjatt&label=Profile%20views&color=0e75b6&style=flat" />
</p>

---

## About

- 🔧 **Building** — [hookfire](https://github.com/Gauravmrjatt/hookfire), a webhook delivery engine in Go: at-least-once delivery, retries with backoff, dead-letter queue, idempotent ingestion, Redis rate limiting, Kubernetes with HPA
- 🧠 **Working in** — Go, PostgreSQL, Redis, RabbitMQ, Kubernetes
- 🎯 **Looking for** — 2027 new-grad Backend / SDE roles
- 👥 **Open to** — open-source collaboration on Go and distributed-systems tooling

---

## Selected work

### Hookfire — webhook delivery engine
A self-hosted webhook delivery engine in Go, in the shape of Svix or Hookdeck. Events are ingested idempotently against a unique key, deliveries are claimed with `FOR UPDATE SKIP LOCKED` by a pool of workers, and failures retry with exponential backoff plus jitter before landing in a dead-letter queue that can be replayed. Requests are HMAC-signed with SSRF checks on the sender, rate limits are enforced per endpoint in Redis, and delivery metrics are exposed to Prometheus. Ships with Kubernetes manifests, an HPA, CI and 10 test files.

`Go` `PostgreSQL` `Redis` `Kubernetes` `Prometheus` `Docker`

[Source](https://github.com/Gauravmrjatt/hookfire)

### Instant Panel — affiliate tracking
An affiliate campaign panel supporting 527K leads from 1.77M tracked clicks at 30% conversion, with INR 2.8 Cr in payments processed. Every query is scoped `token → user → campaign`, so tenants cannot read across accounts. Conversions are idempotent on a unique `(campaign, event, click)` key and pass through ten ordered fraud gates before a lead is credited. Payouts drain through RabbitMQ so a slow gateway never blocks a request, Redis holds the hot reads, and Prometheus scrapes the metrics.

`Next.js` `Express` `MongoDB` `Redis` `RabbitMQ` `Docker`

[Live](https://panel5.logicpay.in) · [Source](https://github.com/Gauravmrjatt/instant-panel)

### Cashbackwallah — multi-carrier logistics
A shipping aggregator: one interface to compare live rates across courier partners, book the cheapest and track the shipment, with a franchise network earning commission on top. 1,700+ orders from about 50 franchise operators, 1,500 of them in a single three-month window. Razorpay payments with signature verification and replay-safe webhooks, KYC-gated ordering and scheduled refunds.

`Next.js` `Express` `Prisma` `PostgreSQL` `Redis` `Razorpay`

[Live](https://cashbackwallah.com) · [Source](https://github.com/Gauravmrjatt/cheapship)

### Codellab — collaborative coding platform
Two people edit the same file through Yjs over WebSockets, then submit to a judge that runs the code inside Docker containers for Node, Python, Java and C++. Each submission gets 0.5 CPU, a 128 MB memory cap, a 64-process limit, no network and a 3-second hard timeout before the container is killed. Contests and live sessions on top.

`Next.js` `Yjs` `WebSocket` `PostgreSQL` `Docker`

[Live](https://codelab.logicpay.in) · [Source](https://github.com/Gauravmrjatt/Codellab)

<details>
<summary><b>More projects</b></summary>

<br/>

| Project | What it does | Notes | |
|---|---|---|---|
| **School** | School management API with Apollo GraphQL and WebSocket subscriptions. Kafka carries attendance, exam and payment events; Redis pub/sub fans results out | 10 Prisma models | [Repo](https://github.com/Gauravmrjatt/School) |
| **OSM Fortress** | Gift code distribution with proof-of-work gating, anti-scraping layers and device fingerprints | 66 routes, 58,000 lines | [Repo](https://github.com/Gauravmrjatt/osm-forest) |
| **TicketHub** | Event ticketing. Book a seat, then an admin approves or rejects the request | 16 endpoints, 5 models | [Live](https://ticket-hub-ten.vercel.app) · [Repo](https://github.com/Gauravmrjatt/TicketHub) |
| **DataVault** | Cloud storage that chunks files into encrypted blobs, with resumable uploads and expiring share links | — | [Live](https://datavault-two.vercel.app) · [Repo](https://github.com/Gauravmrjatt/datavault) |
| **EcoFinds** | Sustainable marketplace with search, cart and checkout | 10 endpoints, 4 models | [Live](https://eco-finds-sage.vercel.app) · [Repo](https://github.com/Gauravmrjatt/EcoFinds) |
| **Telegram bot** | Group management: join approvals, force-join verification, tracked broadcasts | 4 models | [Repo](https://github.com/Gauravmrjatt/tg-bot) |

</details>

---

## Tech

### Languages
<p><img src="https://skillicons.dev/icons?i=go,ts,js,java,python,sql" /></p>

### Backend
<p><img src="https://skillicons.dev/icons?i=nodejs,express,postgres,redis,rabbitmq,mongodb,prisma" /></p>

### Infrastructure
<p><img src="https://skillicons.dev/icons?i=docker,kubernetes,aws,nginx,linux,git,grafana,prometheus" /></p>

### Frontend
<p><img src="https://skillicons.dev/icons?i=react,nextjs,tailwind" /></p>

---

[gauravmrjatt4@gmail.com](mailto:gauravmrjatt4@gmail.com) · [LinkedIn](https://www.linkedin.com/in/gauravmrjatt) · [Portfolio](https://gauravmrjatt.vercel.app) · [Resume](https://gauravmrjatt.vercel.app/resume.pdf)
