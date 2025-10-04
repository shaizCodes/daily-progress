# Day 025 Progress Log

This README summarizes the work done on Day 025, following the daily log convention defined in the root README.

**DATE:** _Monday, September 08, 2025_

**Attendance:** _06:10 PM to 03:04 AM_

## Tasks/Activities

- Studied Google Kubernetes Engine (GKE) and available Kubernetes cluster choices and trade-offs.
- Committed changes to GitHub and built the corresponding Docker image for the application.
- Created Environment Configs and Sessions for the target images.
- Started Sessions on two different clusters; encountered errors on both and resolved the issue on the last cluster.
- Investigated a runtime issue caused by a deprecated Python SQLite wrapper package; researched alternatives and identified APSW (Another Python SQLite Wrapper) as a suitable replacement.

### NPI DB Scraper

- Replaced Express.js with Fastify for improved performance and file-based logging.
- Learned about Pino-Pretty to convert NDJSON logs into human-readable output.
- Implemented P-Limit to parallelize scraping across multiple pages for better resource utilization and faster execution.
- Documented roughly half of the source code using JSDoc conventions and updated repository documentation.

## Tools/Technologies

- Google Kubernetes Engine (GKE)
- Docker
- GitHub (commits/workflows)
- Python (APSW as SQLite wrapper replacement)
- Fastify (replacing Express.js)
- Pino/Pino-Pretty (logging)
- P-Limit (concurrency control)
- JSDoc (documentation)

## Blockers

- Initial cluster errors when starting Sessions on two clusters; resolved on the second cluster. 
- Deprecated Python SQLite wrapper required a replacement; APSW was selected after evaluation.

## Details

- GKE cluster options and trade-offs were reviewed to determine suitable environments.
- Docker images were validated and deployed via commits to GitHub; Environment Configs were created for these images and Sessions were started to test runtime behavior.
- The *** database scraper performance improvements (Fastify, P-Limit) and logging changes (Pino + Pino-Pretty) were aimed at reducing latency and improving log readability. Documentation updates were made using JSDoc for future maintainability.
