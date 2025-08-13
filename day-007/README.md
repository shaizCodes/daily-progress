# Day 006 Progress Log

This README summarizes the work done on Day 007, following the daily log convention defined in the root README.

## Tasks/Activities

- Pulled and explored the *Bitnami WordPress Helm* chart
  - Used `.tgz` archive and `--untar` option to unpack chart folder
  - Installed *WordPress Helm* release with:
    - Default configuration
    - Custom values via `values.yaml`
  - Accessed the release through `minikube service SERVICE_NAME`
  - Rendered chart using helm template and saved output YAML to inspect rendered Kubernetes manifests
- Accepted invitation to *CoderzHunt GitHub* organization for access to private repositories
- Deployed the npidb-scraper project on:
  - *Vercel* (initial attempt stalled due to server listening on port 3000)
  - *AWS EC2* (with help from *Umer*, instance later deleted to conserve credits)
- Set up the scraper environment on *Usama*’s local machine for feedback and alignment with project needs

## Tools/Technologies

- Helm
- Bitnami Wordpress
- Kubernetes (`kubectl` and `minikube`)
- Git/GitHub
- Vercel
- AWS EC2 via SSH
- Node.js (Express, and Puppeteer)

## Blockers

- Vercel deployment stuck: Node.js server running persistently on port 3000 conflicts with Vercel's serverless model
- AWS EC2 instance needed to be removed due to potential credit exhaustion
- Required libraries for Puppeteer were missing on EC2 (libatk, etc.), fixed via manual package installs
- Couldn’t SSH back into EC2 temporarily; resolved by verifying security group settings particularly inbound calls

## Details

- Learned how to render *Helm* charts into *Kubernetes* YAML and understand how values from `values.yaml` are merged into templates
- Plan to modify the `npidb-scraper` server to make it Vercel-compatible (e.g., remove `app.listen`, export as a handler)
- Moving towards a more production-ready structure by validating chart deployment, improving scraper reliability, and integrating feedback from team
