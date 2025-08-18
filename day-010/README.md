# Day 010 Progress Log

This README summarizes the work done on Day 010, following the daily log convention defined in the root README.

**DATE:** _Monday, August 18, 2025_

## Tasks/Activities

- Created a Google email (_[coderzhunt1@gmail.com](mailto:coderzhunt1@gmail.com)_) to utilize free Gemini CLI tool
- Successfully integrated _[Gemini CLI](https://github.com/google-gemini/gemini-cli)_ in VS Code editor for free coding assistance as my free tier Copilot and Cursor expired
- downloaded Python for possible future use
- was assigned a Shakuda platform task, which was to copy the files from monorepo to the remote server via `scp`
  - accessed remote server via `ssh`
  - followed the guidelines to install the Chart



## Tools/Technologies

- Gemini CLI
- Helm
- Secure Shell (`ssh` command)
- Secure Copy (`scp` command)

## Blockers

- installed Gemini CLI globally, but still no terminals recognize the `gemini` command
- release name mismatch of `cephadm` caused installation issues
  - By changing release name from `noble` to `jammy` in `/etc/apt/sources.list.d/ceph.list` file
- faced failure in Shakuda platform `istio/gateway` chart installation due to the version mismatches, which was resolved by falling back to draft-07
  - wrote a bash script function that modified `values.schema.json` after pulling the `istio/gateway` chart by replacing `$defs` with `definitions`, and updating `schema` value


## Details

- Got soaked and late to the office due to rain.
- Received first official task to get hands-on with actual Helm and K8s project
- Two new joines; an Intern, and a Software Engineer
