# Day 022 Progress Log

This README summarizes the work done on Day 022, following the daily log convention defined in the root README.

**DATE:** _Wednesday, September 03, 2025_

**Attendance:** _06:21 PM to 04:10 AM_

## Tasks/Activities

- Created a Docker image that includes DBT Core and specified packages for ELT in a Jupyter environment.
- Built the container locally from the image, then triggered the build through a GitHub workflow.
- Deployed the image to Google Container Registry (GCR) via the GitHub workflow and used the resulting image URI to configure an environment on the platform.
- Created and ran a Session to test the container live in the target environment.
- Opened a GitHub Pull Request with the changes/configuration.

## Tools/Technologies

- Docker
- DBT Core
- Jupyter
- GitHub Actions (workflows)
- Google Container Registry (GCR)
- Platform environment configuration and session runner

## Blockers

- None reported during the session.

## Details

- The image was validated locally before automating the build via CI. After deployment to GCR, the image URI was used to set up an environment configuration on the platform and a live Session was created to test ELT functionality in a Jupyter notebook environment.
- A Pull Request was created to merge the Dockerfile and workflow changes.
