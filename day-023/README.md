# Day 023 Progress Log

This README summarizes the work done on Day 023, following the daily log convention defined in the root README.

**DATE:** _Thursday, September 04, 2025_

**Attendance:** _06:02 PM to 03:39 AM_

## Tasks/Activities

- Had 2 skills assessments: one focused on AWS and another on frontend web development.
- Rebuilt the Environment Configuration for the DBT system on a JupyterHub basic image; the cluster was later shut down.
- Planned to recreate the Session and Environment Configuration in a different cluster, ensuring Python 3.12 is set as the default runtime.

## Tools/Technologies

- JupyterHub image
- DBT (dbt-core and related packages)
- Python 3.12 (target runtime)
- Cloud environment / cluster orchestration

## Blockers

- The original cluster where the Environment Config and Session were built was shut down; Session and EC need to be recreated on a different cluster.

## Details

- Validated the Environment Config locally before deploying to the cluster. After the cluster shutdown, the plan is to rebuild the EC and create a live Session in an alternate cluster, making Python 3.12 the default environment version to ensure compatibility with the DBT and ELT tooling.
