# lt-jobs-scraper

> Daily scraper + data pipeline for developer job ads in Lithuania — clean data in PostgreSQL and weekly skill/salary stats. Python, async httpx, pydantic, typer.

![status](https://img.shields.io/badge/status-in%20progress-yellow) ![area](https://img.shields.io/badge/area-Python-blue) ![license](https://img.shields.io/badge/license-MIT-green)

🚧 **Work in progress.** This repo is part of my public learning roadmap (**Phase 1 — Python & Go foundations**). I build in the open — follow the commits and the roadmap below.

## Why this project

Learn modern, production-style Python on a real problem — and find out which skills Vilnius employers actually ask for.

## What I'm learning

- Modern Python tooling: `uv`, type hints, `ruff`, `mypy`
- Async HTTP with `httpx`, polite scraping (rate limits, robots.txt, retries)
- Data validation with `pydantic`, a CLI with `typer`
- PostgreSQL with SQLAlchemy, idempotent upserts
- Testing with `pytest` and recorded HTTP fixtures
- Scheduled runs with GitHub Actions

## Planned stack

Python 3.12 · uv · httpx · pydantic · typer · SQLAlchemy · PostgreSQL · pytest · GitHub Actions

## Roadmap

- [ ] Project setup: `uv`, `ruff`, `mypy`, `pytest`, CI
- [ ] Scraper for one job site with tests on saved HTML fixtures
- [ ] Normalise jobs (title, company, city, skills, salary) with pydantic models
- [ ] Store in PostgreSQL with de-duplication
- [ ] CLI: `scrape`, `stats`, `export`
- [ ] Add a second and third source
- [ ] Daily GitHub Actions run + weekly stats report (top skills, salary ranges)
- [ ] README: architecture diagram + sample report

## Part of a 10-repo learning roadmap

I'm a full-stack developer in Vilnius ([armansalek.com](https://armansalek.com)) growing into **Python, Go, DevOps, cloud and AI engineering**. These repos connect: the Python and Go services are containerised, deployed and monitored by the DevOps and cloud repos, and the AI projects run on that infrastructure.

| # | Repo | Area | Phase |
|---|---|---|---|
| 1 | **lt-jobs-scraper** (this repo) | Python | 1 |
| 2 | [lt-vocab-api](https://github.com/arman-aru/lt-vocab-api) | Python | 1 |
| 3 | [parcel-locker-api](https://github.com/arman-aru/parcel-locker-api) | Golang | 1 |
| 4 | [go-uptime](https://github.com/arman-aru/go-uptime) | Golang | 1 |
| 5 | [ci-cd-pipelines](https://github.com/arman-aru/ci-cd-pipelines) | DevOps | 2 |
| 6 | [k8s-gitops-lab](https://github.com/arman-aru/k8s-gitops-lab) | DevOps | 2 |
| 7 | [terraform-aws-platform](https://github.com/arman-aru/terraform-aws-platform) | Cloud Computing | 3 |
| 8 | [serverless-media-pipeline](https://github.com/arman-aru/serverless-media-pipeline) | Cloud Computing | 3 |
| 9 | [site-audit-agent](https://github.com/arman-aru/site-audit-agent) | AI Engineering | 4 |
| 10 | [migration-rag-assistant](https://github.com/arman-aru/migration-rag-assistant) | AI Engineering | 4 |

## License

[MIT](LICENSE) © Arman Salek
