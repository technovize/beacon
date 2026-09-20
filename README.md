<div align="center">

<img src="cover.png" alt="The Ascent — One System, Every Architecture" width="320">

# Beacon — companion code for *The Ascent*

**One System, Every Architecture: A Journey from Laptop to Planet-Scale**
by **KC Ramo** · Technovize Publishing

[**Ebook (PDF + EPUB) →**](https://djangozen.com/ebooks/book/the-ascent/)

303 pages · 8.25 × 11 inch · ISBN 978-90-8378-212-6

</div>

---

This repository holds the complete, **MIT-licensed** companion code for *The Ascent*.
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

## License

MIT — free to use in your own projects, personal or commercial, without
attribution. See [`LICENSE`](LICENSE).

The **book text, figures, and cover** are © 2026 KC Ramo / Technovize Publishing
and are not covered by this licence.

---

*Published by Technovize Publishing*
