# Guilherme Andrade

Software engineer based in Lisbon, specialising in Erlang and Elixir.
I've spent over a decade building distributed backend systems —
most recently at Dash Games, before that a decade at Miniclip,
and earlier as a sysadmin at RNL, Técnico Lisboa.

---

## Experience

### Dash Games — Lead Backend Developer · 2023–2026

Sole engineer behind the studio's game backend — from the real-time game server
and player systems to the full GCP infrastructure (Cloud Run, Cloud SQL, GCS,
Secret Manager, IAP, Workload Identity), all under Terraform IaC and CI/CD.
End-to-end ownership across architecture, implementation, deployment and
operations.

### Miniclip — Senior Software Developer · 2013–2023

A decade building, deploying and operating the server-side systems behind some
of Miniclip's biggest titles:

| Title | Backend |
|---|---|
| **8 Ball Pool** (mobile) | 2013–2016 |
| **Agar.io** (web + mobile) | 2016–2018 |
| **Mini Militia** (mobile) | 2018–2020 |
| **Soccer Stars** | 2022 |
| **Mini Pets**, **Dino Pets** | 2013–2014 |

…among others — designing them, shipping them, and keeping them running in
production.

The work spanned the full stack of a real-time game backend:

- **Real-time game servers** — server-authoritative multiplayer for live,
  latency-critical titles, including C++ game servers for real-time multiplayer
  at viral scale. Worked across both major networking models: continuous
  real-time state, and client-side deterministic physics for turn-based titles.
- **Game networking** — Protocol Buffers over TCP/WebSockets as the default
  transport, dropping to UDP for latency-sensitive titles, including a C++
  game-networking library wrapped in an idiomatic Erlang NIF with a custom
  binary protocol.
- **High-concurrency load management** — worker pools, rate limiting and fair
  resource allocation under massive, spiky traffic.
- **Multi-cloud infrastructure** — roughly a decade running game backends on
  AWS at scale (compute, autoscaling, load balancing, managed data stores,
  queues, CDN, infrastructure-as-code). Built demand-driven autoscaling against
  cloud-provider APIs — programmatically launching and tearing down capacity to
  track traffic peaks — across AWS, Linode and DigitalOcean.
- **Edge security under live attack** — automated Cloudflare to shield
  on-demand game servers from DDoS, and built an anti-cheat reputation system
  with trust scoring and graduated reCAPTCHA challenges that withstood a
  large-scale botnet attack shortly after launch.
- **Observability & operations** — production monitoring, alerting and on-call,
  with CI/CD pipelines deploying automatically to production.
- **Runtime-level performance** — native code (NIFs) where the BEAM needed a
  push, plus fixes contributed back upstream into Erlang/OTP itself

### RNL — Técnico Lisboa · Systems Administrator · 2010–2012

Maintained computing and network infrastructure for the university's
student-run IT group.

---

## Open source

A selection of libraries I maintain, mostly for the BEAM ecosystem:

| Project | Description | Stars |
|---|---|---|
| [locus](https://github.com/g-andrade/locus) | MMDB reader for Erlang/Elixir — IP geolocation and ASN lookup | ⭐ 121 |
| [sqids-elixir](https://github.com/sqids/sqids-elixir) | Official Elixir port of Sqids — short unique IDs from numbers | ⭐ 94 |
| [aequitas](https://github.com/g-andrade/aequitas) | Fairness regulator and rate limiter | ⭐ 50 |
| [backwater](https://github.com/g-andrade/backwater) | Intercluster RPC for Erlang and Elixir | ⭐ 48 |
| [taskforce](https://github.com/g-andrade/taskforce) | On-demand worker pools for parallelizable tasks | ⭐ 43 |
| [maestro](https://github.com/g-andrade/maestro) | Pool of pools | ⭐ 31 |
| [deigma](https://github.com/g-andrade/deigma) | Event sampler | ⭐ 24 |
| [tls_certificate_check](https://github.com/g-andrade/tls_certificate_check) | CA store and partial chain handler for TLS | ⭐ 23 |

→ [full list](https://github.com/g-andrade?tab=repositories)

---

## Upstream contributions

**[erlang/otp](https://github.com/erlang/otp)**

- `ets:select_replace/2` — matchspec-based row replacement in ETS tables
- `math:fmod/2` — floating-point modulo BIF
- `enif_hash` — hashing arbitrary terms from NIF code
- Cryptographically strong random number generation via `rand` plugin
- `zlib` inflation dictionary extraction
- Various fixes and documentation improvements

**Erlang/Elixir ecosystem**

[rebar3](https://github.com/erlang/rebar3),
[rebar3_hex](https://github.com/erlef/rebar3_hex),
[rebar3_hank](https://github.com/AdRoll/rebar3_hank),
[ex_doc](https://github.com/elixir-lang/ex_doc),
[exile](https://github.com/akash-akya/exile),
[hackney](https://github.com/benoitc/hackney),
[certifi](https://github.com/certifi/erlang-certifi),
and [others](https://github.com/search?q=author%3Ag-andrade+is%3Apr+is%3Amerged&type=pullrequests)

---

## Experiments

Small interactive toys — audio illusions, optics, generative graphics:

- [Circles](https://www.gandrade.net/circles/) — generative canvas animation with live controls
- [Coalescence](https://www.gandrade.net/coalescence/) — audio-reactive canvas visualisation
- [Curvature blindness](https://www.gandrade.net/curvature_blindness/) — the curvature-blindness optical illusion, rendered live
- [Shepard tone](https://www.gandrade.net/shepard/) — the auditory illusion of a pitch that seems to climb forever
- [Teardrop](https://www.gandrade.net/teardrop/) — generative canvas animation that responds to mouse movement
- [WebGL plotter](https://www.gandrade.net/webgl-plot/) — plots mathematical formulas in WebGL

---

## Talks

[erlchronos](https://www.gandrade.net/talks/erlchronos_euc2016/) — a gen_server wrapper with ticks (Erlang User Conference 2016)

---

## Technologies

**Languages** — Erlang, Elixir, SQL, C++; some C, JavaScript, Python, Rust over the years

**Runtime / frameworks** — OTP, Cowboy, Phoenix (LiveView), Ecto, Protocol Buffers

**Infrastructure** — GCP and AWS; Terraform, CloudFormation, Docker; demand-driven autoscaling via cloud-provider APIs

**Data** — PostgreSQL, DynamoDB, Redis

**Observability & CI/CD** — Datadog, OpenTelemetry, PagerDuty; GitHub Actions, Jenkins, CodeDeploy

---

## Contact

[website@gandrade.net](mailto:website@gandrade.net) ·
[LinkedIn](https://www.linkedin.com/in/guilhermemandrade/) ·
[Website](https://www.gandrade.net)
