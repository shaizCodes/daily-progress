# Daily Progress Tracker (Archived)

This repository is an archival, read-only personal log of a developer's first job experience. It documents daily work, learning, and blockers across multiple stacks and projects. Each day is recorded in its own folder (for example `day-001/`, `day-002/`, ...), with a short summary of activities, tools used, and any challenges encountered.

Important notes
---------------
- Read-only archive: This repository is intended as a historical record. It has been archived for public reading only — no interactions (issues, PRs, or edits) are expected or required.
- Not a codebase: The repository contains notes and small examples for illustration. It is not a production code repository and should not be treated as an installable project.
- Personal diary: Entries reflect personal experiences, troubleshooting, and lessons learned. They are written for personal reference and to help others learning similar topics. The content is not intended to blame or defame any individual or organization.

Personal note
-------------
These entries were written primarily for my own record. During this period I was working night shifts which disrupted my sleep and affected my ability to keep up with writing at a steady pace. When time became scarce I copied and adapted my daily scrum notes into these files so I could finish the log and share my experience. This is a personal diary — not a marketing effort — and I included these notes in the hope they help others who might be learning similar tools and problems.

What you'll find here
---------------------
- Day-by-day summaries describing tasks, tools/technologies, blockers, and key details.
- Short notes on debugging sessions, development setups, and small snippets used for illustration. Major projects and private source code are intentionally excluded.
- Practical learnings from real work: debugging techniques, environment setup, CI/CD observations, quick fixes, and small refactors.

Key takeaways and learnings
---------------------------
- Debugging and tooling: Hands-on use of IDE debuggers, headless browser automation (Puppeteer), and container workflows improved problem diagnosis and reduced iteration time.
- Resource management: Migrating from heavier workflows (duplicating browser profiles, using deprecated libraries) to resource-efficient patterns avoided memory and stability issues.
- Automation and concurrency: Implementing semaphores, queues, and controlled parallelism helped scale small automation tasks while preserving system stability.
- Documentation habit: Keeping daily notes made it easier to capture decisions, regressions, and follow-ups — useful for onboarding and troubleshooting later.

If you found this useful
-----------------------
- Feel free to read and learn from the entries. If you want to preserve a copy, clone the repo locally.
- I do not expect PRs or issues on this archive. If you need to reach me about the contents, use my public contact channels (lookup the profile page).

License and code
----------------
- This repository contains primarily diary-style documentation and a few illustrative snippets. It does not include production code. Use the content for personal learning or educational purposes; attribution is appreciated.

----

Original convention (kept for reference)
---------------------------------------
Each daily folder (e.g., `day-001/`, `day-002/`, ...) contains a `README.md` that follows this structure:

- **Tasks/Activities:** List what was done, learned, or practiced
- **Tools/Technologies:** Mention software, frameworks, or platforms used
- **Blockers:** Note any issues or challenges encountered
- **Details:** Add extra notes or context as needed

This convention was used to ensure consistency and to make it easy to track progress across different technologies and irregular tasks.

How to navigate this archive
----------------------------
- Browse `day-XXX/README.md` files in chronological order to follow the full timeline.
- Each day file contains a short summary, tools used, blockers, and details — start with the day's header and the "Tasks/Activities" section for the main actions taken.
- Use search (repository search or your code editor) to find topics such as "Puppeteer", "GKE", "DBT", "NestJS", or "Chrome extension".

Major topics covered (high level)
---------------------------------
- Browser automation and extensions: Puppeteer-based automation, Chrome extension development, tab/session management, and concurrency controls (semaphores/queues).
- Containers and CI/CD: Docker image builds, GitHub Actions workflows, container registries, and validating images in test environments.
- Cloud orchestration: Google Kubernetes Engine (GKE) cluster setup, environment configuration, and cluster troubleshooting.
- Data engineering / ELT: dbt/dbt-core packaging and building container images for Jupyter/ELT workflows.
- Backend development: NestJS, TypeORM, PostgreSQL, DTOs, auth guards, custom decorators, migrations and raw SQL queries.
- Storage/infra components: MinIO object storage validation and related session tests.
- Logging and observability: NDJSON logging, Pino + Pino-Pretty, Prometheus and Helm chart patches.
- Dependency migrations and fixes: replacing deprecated libraries (e.g., PhantomJS → Puppeteer, older SQLite wrappers → APSW) to improve maintainability.
- Productivity & AI-assisted coding: use of Cursor and ChatGPT to scaffold code and UI; notes discuss where generated code needed manual fixes.

Scope and limitations
---------------------
- This repository is a personal diary and learning log. It contains summaries, notes, and small illustrative snippets, but it is not a packaged project or an installable codebase.
- Sensitive or proprietary source code and internal project details are intentionally excluded. The content avoids blaming or defaming individuals or organizations.

If you want more
----------------
- I can generate a compact JSON index of day entries (date + one-line summary) for easy searching. Say "yes" and I'll create it.
- I can also produce a short one-line repository description suitable for the GitHub repo metadata.

----

Thank you for reading. I archived this log to preserve the learning trail and to make it available as a helpful reference for others studying similar topics.
