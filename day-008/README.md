# Day 008 Progress Log

This README summarizes the work done on Day 008, following the daily log convention defined in the root README.

**DATE:** _Thursday, August 14, 2025 (**public holiday - PK Independence day**)_

**Attendance:** _06:09 PM to 03:05 AM_

## Tasks/Activities

- documented scraper source code, and refactored it to some extent with minor bug fixes
- added support for CSV file creation and wrote records instantly rather than in batches at the end
- set up the project on client's machine and adapted it based on his reviews
- revised and practiced Kubernetes concepts watching the suggested YouTube crash course, *[Kubernetes Tutorial for Beginners [FULL COURSE in 4 Hours]](https://www.youtube.com/watch?v=X48VuDVv0do&t=5557s)*

## Tools/Technologies

- JavaScript
- Node.js
- Docker Desktop
- MiniKube (`minikube`, and `kubectl`)
- `k9s`

## Blockers

- None

## Details

- Labels are used to classify and identify the Kubernetes resources.
- Services connect to pods via selectors matching the pod labels.
- The target ports in services represent container ports of pods, and they must match for connection.
- A pod can have multiple containers, and their environment variables values should come from ConfigMaps and Secrets.
- ***Officially, I had two off days (`13/08`, and `14/08`), but here I was still.😁***
