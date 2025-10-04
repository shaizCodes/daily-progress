# Day 028 Progress Log

This README summarizes the work done on Day 028, following the daily log convention defined in the root README.

**DATE:** _Thursday, September 11, 2025_

**Attendance:** _06:10 PM to 03:20 AM_

## Tasks/Activities

- Explored Dandified Yum (`dnf`) for managing packages on Oracle Linux.
- Switched to the `yum` package manager for consistency and broader community support to resolve package-related bugs.
- Reset and rebooted the Google Cloud Compute Engine VM to ensure packages required for platform deployment were tracked and available.
- Refactored and optimized the installation script for improved readability and maintainability.

xxx
- 1 hour English speaking training...

## Tools/Technologies

- Oracle Linux package managers (`dnf`, `yum`)
- Google Cloud Compute Engine (GCE)
- Shell scripting

## Blockers

- No critical blockers; package manager selection needed verification across environments.

## Details

- `dnf` was tested but then reverted to `yum` due to compatibility and support considerations. The installation script was updated to reflect the package manager choice and to make maintenance easier.
- A VM reboot ensured the environment state was clean before running the installation script.
