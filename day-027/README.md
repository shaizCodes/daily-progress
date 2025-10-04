# Day 027 Progress Log

This README summarizes the work done on Day 027, following the daily log convention defined in the root README.

**DATE:** _Wednesday, September 10, 2025_

**Attendance:** _06:10 PM to 03:50 AM_

## Tasks/Activities

- Received access to a Google Cloud Compute Engine VM running Oracle Linux 9.
- Upgraded the OS build to Oracle Linux 9.6 to meet task requirements.
- Refactored the platform installation script to support Oracle Linux 9.x in addition to Ubuntu 20.x.x.
- Resolved package availability issues by adding conditionals to use the DNF package manager on Oracle Linux 9.6.
- Applied patches for Prometheus and Helm chart specification validation.
- [TODO] Verify the script works as expected, then create a Pull Request.

## Tools/Technologies

- Google Cloud Compute Engine (GCE)
- Oracle Linux 9.6
- Ubuntu 20.x.x
- DNF package manager
- Prometheus
- Helm

## Blockers

- None reported; next step is verification and PR creation.

## Details

- The installation script now detects the OS family and selects the appropriate package manager and installation steps. Patches were applied to address Prometheus and Helm chart validation issues encountered during the installation process.
- After verification in the target environment, the next step is to open a PR with the updated script and patches.
