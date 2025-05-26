**Why System Design matters**

* Gatekeeper round for SD-II/III, tech-lead, and architect roles.
* Tests ability to craft *robust, scalable, cost-aware* solutions—not just write code.

**Two pillars**

| HLD (Architecture)                           | LLD (Code)                                             |
| -------------------------------------------- | ------------------------------------------------------ |
| What components you need & how they interact | Exact classes, APIs, DB schema, concurrency primitives |
| No code—just diagrams & trade-offs           | Compilable code or close pseudo-code                   |

**HLD Roadmap (12 checkpoints)**

1. **Infrastructure Basics** – serverless vs EC2, vertical vs horizontal scaling.
2. **Data Stores** – SQL, NoSQL, in-memory; replication, partitioning, sharding.
3. **Consistency Models** – eventual, quorum, causal; CAP theorem.
4. **Caching & CDNs** – Redis, Memcached, LFU/LRU; CDN placement.
5. **Networking 101** – TCP/UDP, HTTP versions, WebSockets/WebRTC.
6. **Load Balancing** – round-robin, least-connections, consistent-hashing, reverse-proxy.
7. **Message Queues** – Kafka, RabbitMQ; pub-sub and async workflows.
8. **Monolith → Microservices** – containers, Docker, single-point-failure, graceful migration.
9. **Observability** – logging, metrics, alerts, Prometheus, Grafana.
10. **Security** – OAuth, ACLs, TLS, encryption at rest & in transit.
11. **Trade-offs Grid** – push vs pull, availability vs consistency, latency vs throughput.
12. **Deliberate Practice** – design Netflix, WhatsApp, Twitter, Uber, YouTube, Instagram, Zoom, Amazon, etc.

**LLD Roadmap (8 checkpoints)**

1. OOP pillars (encapsulation, abstraction, inheritance, polymorphism).
2. SOLID principles (SRP, OCP, LSP, ISP, DIP).
3. Design patterns (Factory, Singleton, Adapter, Observer, Strategy, etc.).
4. Concurrency & thread-safety (locks, atomic ops, producer-consumer).
5. UML diagrams (class, sequence, component) – optional but good.
6. API craft (resource naming, versioning, REST vs gRPC, pagination).
7. Clean-code discipline (small classes, DRY, no “God” objects).
8. Hands-on problems (Tic-Tac-Toe, Chess, URL shortener, notification service).

**Suggested Practice Order**

1. Tic-Tac-Toe (LLD warm-up)
2. URL Shortener (HLD + small LLD)
3. WhatsApp messaging (queues, caching)
4. Instagram feed (fan-out, cache, CDN)
5. Uber (real-time matching, geo partitions)
6. Zoom (WebRTC, media servers)
7. Netflix (full checklist)

**Realistic timeline**

* **Experienced dev** – 2–3 months (revise & drill).
* **New to most topics** – 4–6 months (learn, build mini-projects, drill).

---

### What to do next

1. **Pick one system each week** from the practice list—sketch HLD in 30 min, then critique your design for trade-offs.
2. **Pair up**: explain your design to a friend/colleague; field their “why not X?” questions.
3. **Build small POCs**—e.g., integrate Redis cache into an existing side-project, deploy a Dockerised microservice.
4. **Track concepts**: keep a cheat-sheet of pros/cons (SQL vs NoSQL, LRU vs LFU, etc.).
5. **Mock interviews** after 4–6 full designs.

Feel free to ask if you’d like a deeper dive or standalone guide on any specific bullet above!

## Resources:
**System Design:** https://www.youtube.com/watch?v=CuQmQpvw04I
