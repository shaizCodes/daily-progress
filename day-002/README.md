# Day 002 Progress Log

This README summarizes the work done on Day 002, following the daily log convention defined in the root README.

**DATE:** _Wednesday, August 06, 2025_

**Attendance:** _06:04 PM to 03:05 AM_

## Tasks/Activities
- Created a GitHub account ([shahzad-coderzhunt](https://github.com/shahzad-coderzhunt)) using official email ([m.shahzad@coderzhunt.com](mailto:m.shahzad@coderzhunt.com)) and synced it in VS Code
- Installed and explored the [Kubernetes](https://marketplace.visualstudio.com/items?itemName=ms-kubernetes-tools.vscode-kubernetes-tools) VS Code extension to understand Kubernetes architecture by building sample clusters, deployments, and services with `kubectl`. Used the Minikube dashboard for hands-on experience
- Installed [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens), [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker), and [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) VS Code extensions for future productivity
- Reviewed and explained a new GitHub Issue regarding GPT-OSS integration for the *Shakuda* platform:
    - Proposed creating a Pull Request to support the [GPT-OSS](https://openai.com/index/introducing-gpt-oss/) model under Ollama models, managing deployment via Helm chart and Google Kubernetes Engine
    - Noted the need for backward compatibility and documentation of any failures for legacy model troubleshooting
- Continued practicing Kubernetes and Minikube
- Attempted web scraping of the National Provider Identifier ([npidb.org](https://npidb.org/doctors/allopathic_osteopathic_physicians/allergy_207ka0200x)) website using Python:
    - Created Python scripts to read sample pages
    - Tried bypassing Cloudflare protection using Selenium, Undetected ChromeDriver, and Playwright
    - Researched solutions on Stack Overflow, official documentation, ChatGPT, and Claude

## Tools/Technologies
- GitHub
- VS Code
- Kubernetes VS Code extension
- GitLens VS Code extension
- Docker VS Code extension
- Remote Development VS Code extension
- Kubernetes
- Minikube
- Python
- Selenium
- Undetected ChromeDriver
- Playwright
- Helm
- Google Kubernetes Engine

## Blockers
- Unable to bypass Cloudflare protection on *** using Selenium and Undetected ChromeDriver

## Details
- Used Kubernetes VS Code extension and Minikube dashboard for practical understanding of clusters, deployments, and services
- Installed productivity extensions (GitLens, Docker, Remote Development) for future use
- The GPT-OSS integration task involved supporting a new model in Ollama via Helm and GKE, with documentation of any failures for legacy model troubleshooting
- Multiple web scraping solutions were tested and researched, but none succeeded for npidb.org (some worked for other sites)
