<div align="center">

```
██████╗ ██╗   ██╗███████╗████████╗
██╔══██╗██║   ██║██╔════╝╚══██╔══╝
██████╔╝██║   ██║███████╗   ██║
██╔══██╗██║   ██║╚════██║   ██║
██║  ██║╚██████╔╝███████║   ██║
╚═╝  ╚═╝ ╚═════╝ ╚══════╝   ╚═╝
```

### Issatay Tokpakbayev · Backend Engineer
**Rust · Low-Latency · Web3 · Almaty, KZ**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/issatay-tokpakbayev-305b86280/)
[![Open to Work](https://img.shields.io/badge/Open%20to%20Work-Remote%20Rust%20Roles-16a34a?style=flat-square)](mailto:)

</div>

---

## Who I Am

I write Rust for systems where latency is measured in microseconds and correctness isn't optional.

By day I'm building low-latency trading infrastructure at **KASE** (Kazakhstan Stock Exchange) — FFI wrappers over Aeron IPC, high-throughput market data feeds, zero-copy pipelines. Before that I shipped real-time Rust microservices at scale at a game studio, and before that I integrated blockchain APIs in C#/.NET at Altyn Bank.

I also have production **Solana** smart contract experience, and I've spent enough time in the HFT trenches to care deeply about things like memory allocator behavior and kernel bypass networking.

Currently looking for **remote mid/senior Rust or backend roles** — trading infrastructure, systems, Web3, or anywhere the work is genuinely hard.

---

## What I'm Building

### [e-shop](https://github.com/kusetos/e-shop) — Microservices E-Commerce in Rust

> Production-style e-commerce backend. Not a tutorial. An actual reference architecture.

5 independent services, all in Rust — API Gateway, Catalog, Basket, Ordering, Identity. Event-driven via Kafka. JWT auth with Argon2. Compile-time checked SQL via `sqlx`. Deployable on Docker Compose or Kubernetes (Minikube).

```
Stack: Axum · Tokio · sqlx · rdkafka · PostgreSQL · Redis · Kafka · Docker · K8s
```

The architecture is intentional: prices are fetched server-side from Catalog so the client can never manipulate them. Stock is decremented asynchronously via `order-created` Kafka events. The gateway validates JWT and injects `x-user-id` so downstream services never touch auth logic.

---

## Tech I Reach For

```rust
let stack = vec![
    "Rust (async, unsafe, FFI, macros)",
    "Axum / Actix-web / Tokio",
    "PostgreSQL + sqlx",
    "Apache Kafka / rdkafka",
    "Redis",
    "Solana / Anchor",
    "Docker / Kubernetes",
    "Aeron IPC",
    "C# / .NET (previous life)",
];
```

---

## Background

```
2024 – now   Backend Engineer @ KASE (HFT infra, Aeron IPC, market data feeds)
2023 – 2024  Rust Engineer @ GMG (real-time microservices at scale)
2022 – 2023  Backend Developer @ Altyn Bank (C#/.NET, blockchain APIs)
```

I'm also a **KBTU** (Kazakh-British Technical University) student — which means I spend my weekends alternating between reading papers on cognitive science and debugging `rdkafka` consumer group offsets.

---

## What I'm Exploring

- Database internals — building one from scratch in Rust (inspired by [ToyDB](https://github.com/erikgrinaker/toydb))
- AI/ML infrastructure — my low-latency background maps well to inference serving and GPU kernel work
- CUDA/Triton → eventually `cuda-oxide`

---

<div align="center">

**Currently open to remote Rust / backend roles.**
Build something fast with me.

[![LinkedIn](https://img.shields.io/badge/Let%27s%20connect-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/issatay-tokpakbayev-305b86280/)

</div>
