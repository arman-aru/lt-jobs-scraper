# lt-jobs-scraper

> Daily scraper + data pipeline for developer job ads in Lithuania — clean data in PostgreSQL and weekly skill/salary stats. Python, async httpx, pydantic, typer.

![status](https://img.shields.io/badge/status-in%20development-yellow) ![license](https://img.shields.io/badge/license-MIT-green)

## Overview

A data pipeline that collects developer job ads from Lithuanian job sites every day, cleans and de-duplicates them, stores them in PostgreSQL and produces weekly statistics on the most requested skills and salary ranges.

## Features

- Scrapers for multiple Lithuanian job sites, with rate limiting, retries and robots.txt respect
- Normalised job records: title, company, city, skills, salary range, posting date
- De-duplication across sources with idempotent upserts
- Command-line interface: `scrape`, `stats`, `export`
- Weekly report of top skills and salary ranges (Markdown and CSV)
- Scheduled daily runs with GitHub Actions

## Tech stack

Python 3.12 · uv · httpx · pydantic · typer · SQLAlchemy · PostgreSQL · pytest · GitHub Actions

## License

[MIT](LICENSE) © Arman Salek
