# Day 006 Progress Log

This README summarizes the work done on Day 006, following the daily log convention defined in the root README.

**DATE:** _Tuesday, August 12, 2025_

## Tasks/Activities
- Created a Docker account (synced with official email and GitHub)
- Enabled MFA/2FA using Google Authenticator for GitHub and Docker accounts
- Created a public repository for hands-on Helm, *[practice-Helm](https://github.com/shahzad-coderzhunt/practice-Helm)*
- Made the *[daily-progress](https://github.com/shahzad-coderzhunt/npidb-scraper)* repository public
- Created a new private repository for *[npidb-scraper](https://github.com/shahzad-coderzhunt/practice-Helm)* and shared it with PM
- Practiced Helm commands using official documentation
- Learned to:
  - Add repositories, search charts (globally and specific), and pull charts
  - Install charts, list releases (including uninstalled), uninstall releases, and track their status
  - View release history and show chart values
- Installed `k9s` and practiced key bindings to get familiar
- Pulled and installed `ingress-nginx` from ArtifactHub and accessed it via Minikube

## Tools/Technologies
- Helm
- ingress-nginx (ArtifactHub)
- k9s
- Kubernetes / Minikube
- GitHub
- Docker

## Blockers
- None noted

## Details
- Security hardening: Enabled MFA across GitHub and Docker
- Helm ops practiced included repository management, chart discovery, installation lifecycle, history inspection, and values inspection
- `k9s` used for cluster navigation to reinforce Kubernetes concepts
- `ingress-nginx` installed and verified reachable through Minikube

### Helm Commands Practiced (examples)

```bash
# Add a Helm repository and update repo cache
helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update

# Search charts (global and specific)
helm search hub nginx
helm search repo bitnami/nginx

# Pull a chart and inspect default values
helm pull bitnami/nginx --untar
helm show values bitnami/nginx | head -n 40 | cat

# Install, list (including uninstalled), history, rollback, uninstall
helm install my-nginx bitnami/nginx
helm list
helm list --all
helm history my-nginx
helm rollback my-nginx 1
helm uninstall my-nginx
```

### Minikube + ingress-nginx (quick demo)

```bash
# Start Minikube
minikube start

# Enable or install ingress-nginx (two common approaches)
minikube addons enable ingress
# or via Helm
helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
helm repo update
helm install ingress-nginx ingress-nginx/ingress-nginx --namespace ingress-nginx --create-namespace

# Verify controller is running
kubectl get pods -n ingress-nginx

# Access via Minikube tunnel or service
minikube tunnel &
kubectl get svc -n ingress-nginx | cat
```


