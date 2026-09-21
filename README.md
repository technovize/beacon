<div align="center">

<img src="cover.png" alt="The Ascent — One System, Every Architecture" width="320">

# Beacon — companion code for *The Ascent*

**One System, Every Architecture: A Journey from Laptop to Planet-Scale**
by **KC Ramo** · Technovize Publishing

[**Ebook (PDF + EPUB) →**](https://djangozen.com/ebooks/book/the-ascent/) · [**Paperback →**](https://www.amazon.com/dp/9083782123)

303 pages · 8.25 × 11 inch · ISBN 978-90-8378-212-6

</div>

---

This repository holds the complete companion code for *The Ascent*.
It is the source for **Beacon**, the fictional collaborative knowledge platform the
book follows from a single Django process on a laptop all the way to a planet-scale
distributed system serving millions of users across six continents.

<sub>The short address <code>technovize.com/code/ascent</code> printed in the book redirects here.</sub>

## About the book

Every chapter opens with one scaling crisis, explains why it happened as a
consequence of the previous chapter's success, and works through the fix with
real code and real trade-offs. Unlike survey-style system-design books that jump
between ten products, *The Ascent* tells a single continuous story: the code
evolves, the architecture deepens, the patterns compound.

## What's in this repository

The code is organized by chapter. Each chapter's directory contains Beacon as it
stands at the **end** of that chapter, so you can read the book with the matching
code open beside it, or diff one chapter against the next to see exactly what a
scaling decision changed.

| Part | Chapters | The climb |
|---|---|---|
| I — The Monolith | 1–4 | One server, the first users, caching, the monolith under load |
| II — Distribution Begins | 5–8 | Replicas, sharding, services, asynchronous work |
| III — Real Time and Real Big | 9–12 | Collaboration, search, the feed, analytics |
| IV — Planetary Scale | 13–16 | Multi-region, observability, cost, the principles that remain |

## Repository layout

Each chapter directory holds Beacon as it stands at the **end** of that chapter,
so you can read with the matching code open beside you — or diff one chapter
against the next to see exactly what a scaling decision changed. 640 files across
sixteen chapters; the count grows with the system.

| # | Directory | Chapter | Files |
|---|---|---|---|
| 1 | [chapter-01](chapter-01/) | A Single Server and a Dream | 19 |
| 2 | [chapter-02](chapter-02/) | The First Thousand Users | 20 |
| 3 | [chapter-03](chapter-03/) | Caching Everything That Moves | 21 |
| 4 | [chapter-04](chapter-04/) | The Monolith Groans | 26 |
| 5 | [chapter-05](chapter-05/) | Read Replicas and the Split Brain | 28 |
| 6 | [chapter-06](chapter-06/) | Sharding Beacon's Knowledge Graph | 33 |
| 7 | [chapter-07](chapter-07/) | The Monolith Becomes a Service | 46 |
| 8 | [chapter-08](chapter-08/) | Async Work and the Message Bus | 43 |
| 9 | [chapter-09](chapter-09/) | Collaboration at the Speed of Light | 47 |
| 10 | [chapter-10](chapter-10/) | Search Across a Billion Documents | 50 |
| 11 | [chapter-11](chapter-11/) | The Feed That Never Sleeps | 42 |
| 12 | [chapter-12](chapter-12/) | Data Lakes and the Analytical Sidecar | 46 |
| 13 | [chapter-13](chapter-13/) | Going Multi-Region | 70 |
| 14 | [chapter-14](chapter-14/) | Observability When Things Go Dark | 64 |
| 15 | [chapter-15](chapter-15/) | The Cost of Scale | 44 |
| 16 | [chapter-16](chapter-16/) | The Principles That Remain | 41 |

## Quick start

Clone the repository linked from `technovize.com/code/ascent`, then, from the
project root:

```bash
cd chapter-01
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Later chapters add services and infrastructure; each chapter's `README` lists
what it needs and how to run it.

## A note on the code

The listings are **illustrative** — they show the shape of each solution as the
book teaches it, not a hardened, production-ready system. The commands run in
order; they are not idempotent scripts. Read them alongside the chapter that
introduces them.

## Licence

The **Companion Code License** — build with it, learn from it, use it in your own
work; just don't republish the book or this code as your own.
See [`LICENSE`](LICENSE).

GitHub shows this as `NOASSERTION`, which is expected: it is a custom licence,
not a missing one.

The **book text, figures, and cover** are © 2026 KC Ramo / Technovize Publishing
and are not covered by it.

---

*Published by Technovize Publishing*
