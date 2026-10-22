# Gaurav Chaudhary

Full-stack engineer working in TypeScript, Next.js and Node.
I build the whole thing: schema, API, interface, deploy.

[Portfolio](https://gauravmrjatt.vercel.app) · [Resume](https://gauravmrjatt.vercel.app/resume.pdf) · [LinkedIn](https://www.linkedin.com/in/gauravmrjatt) · [Email](mailto:gauravmrjatt4@gmail.com)

---

## Selected work

### Instant Panel
An affiliate campaign panel, about 31,000 lines. Campaign tracking, lead management and payout runs. Payouts drain through a RabbitMQ queue so a slow payout never blocks the request, Redis holds the hot reads, and Prometheus scrapes the metrics. 107 endpoints, 12 models, 10 test files.

`Next.js` `Express` `MongoDB` `Redis` `RabbitMQ` `Docker`

[Source](https://github.com/Gauravmrjatt/instant-panel)

### Cashbackwallah
A logistics and shipping platform, about 59,000 lines. A customer prices a shipment, creates an order and tracks it. A franchise network sits on top, earning referral commission and requesting withdrawals. Razorpay handles the payments. 145 endpoints and 23 Prisma models behind a Next.js 16 client.

`Next.js` `Express` `Prisma` `PostgreSQL` `Razorpay`

[Source](https://github.com/Gauravmrjatt/cheapship)

### Codellab
A collaborative coding platform. Two people can edit the same file at once through Yjs over WebSockets, then submit to a judge that runs the code inside Docker containers for Node, Python, Java and C++. About 32,000 lines, 23 routes, contests and live sessions.

`Next.js` `Yjs` `WebSocket` `PostgreSQL` `Docker`

[Source](https://github.com/Gauravmrjatt/Codellab)

### School
A school management API. Apollo GraphQL with WebSocket subscriptions over 10 Prisma models covering students, attendance, exams and fee invoices. Kafka carries attendance, exam result and payment events, and Redis pub/sub fans results out to whoever is subscribed.

`TypeScript` `Apollo` `Prisma` `PostgreSQL` `Redis` `Kafka`

[Source](https://github.com/Gauravmrjatt/School)

<details>
<summary><b>More projects</b></summary>

<br/>

| Project | What it does | Numbers | |
|---|---|---|---|
| **TicketHub** | Event ticketing. Book a seat, then an admin approves or rejects the ticket request | 16 endpoints, 5 models | [Live](https://ticket-hub-ten.vercel.app) · [Repo](https://github.com/Gauravmrjatt/TicketHub) |
| **DataVault** | Cloud storage that chunks files into Telegram channels, so capacity follows the channel rather than a paid bucket | 80 components | [Live](https://datavault-two.vercel.app) · [Repo](https://github.com/Gauravmrjatt/datavault) |
| **OSM Fortress** | Gift code distribution with proof of work gating, anti scraping layers and device fingerprints | 66 routes, 58,000 lines | [Repo](https://github.com/Gauravmrjatt/osm-forest) |
| **EcoFinds** | Sustainable marketplace with search, cart and checkout | 10 endpoints, 4 models | [Live](https://eco-finds-sage.vercel.app) · [Repo](https://github.com/Gauravmrjatt/EcoFinds) |
| **Telegram bot** | Group management: join approvals, force join verification, tracked broadcasts | 4 models | [Repo](https://github.com/Gauravmrjatt/tg-bot) |
| **Tod AI** | Alphabet game for toddlers with phonetic audio | 45 components | [Live](https://tod-ai-teal.vercel.app) · [Repo](https://github.com/Gauravmrjatt/tod-ai) |

</details>

---

## Currently

- Building Instant Panel, mostly the payout side
- Learning distributed systems properly: queues, idempotency, what happens when a consumer dies mid batch
- Open to full-stack and backend roles

<sub>Last updated: October 2026</sub>

---

## Stack

**Languages** TypeScript · JavaScript · Python · SQL · Java

**Frontend** React · Next.js · Tailwind CSS · shadcn/ui · MUI · Zustand · TanStack Query

**Backend** Node.js · Express · Apollo GraphQL · Payload CMS · REST · WebSocket · JWT

**Data** PostgreSQL · Prisma · MongoDB · Redis

**Infra** Docker · RabbitMQ · Kafka · Prometheus · Nginx · Vercel

---

## Let's talk

Happy to talk about full-stack work, backend design, or anything queue-shaped.

[gauravmrjatt4@gmail.com](mailto:gauravmrjatt4@gmail.com) · [LinkedIn](https://www.linkedin.com/in/gauravmrjatt) · [Portfolio](https://gauravmrjatt.vercel.app)
