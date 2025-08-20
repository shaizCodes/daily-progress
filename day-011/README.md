# Day 011 Progress Log

This README summarizes the work done on Day 011, following the daily log convention defined in the root README.

**DATE:** _Tuesday, August 19, 2025_

## Tasks/Activities

- accessed remote server (interview.canopyhub.io) where the test cluster is deployed
- worked on pending AIO deployment script
  - created a Pull Request with a fix for istio/gateway chart schema validation
  - updated the AIO_install.sh file to deploy target repository charts. i.e., prometheus, certmanager, etc.
  - succeeded running the AIO_install.sh that fetches target charts, modifies Istio/gateway schema validation, and installs Prometheus, CertManager, and a few Istio charts
- Had Scrum stand up as usual reporting previous day progress and blockers

## Tools/Technologies

- Helm (`helm`)
- Secure Shell (`ssh` command)
- Secure Copy (`scp` command)
- Kubernetes (`kubectl`)

## Blockers

- [x] failed to deploy Istio Gateway due to failing schema validation [RESOLVED]
- [x] failed to deploy Prometheus due to misconfigured role bindings [RESOLVED]

## Details

- wrote a Bash script function that replaces a few target words in `values.schema.json` file to temporarily fix the Istio/gateway installation issues (version, and keyword changes)
