# Day 009 Progress Log

This README summarizes the work done on Day 009, following the daily log convention defined in the root README.

## Tasks/Activities

- Set up *NGINX* (pronounced as "engine X") server on *Windows* locally to understand how it works.
- Configured *NGINX* to act as a reverse proxy, forwarding requests from `localhost:80` to a backend server at `localhost:3000/scrape`.
- Attempted to create a *Git* server on a *Windows* machine.
  - Ran a cleanup script suggested by *ChatGPT* to undo partial *Git* server setup.
  - Unfortunately, this led to deletion of user account data and eventually the removal of the user account out of frustration.😒

## Tools/Technologies

- Nginx (on Windows 11)
- Git

## Blockers

- None encountered in the NGINX setup
- Faced data loss while trying to set up a Git server manually on Windows

## Details

- The motivation behind trying Nginx setup was to get a proper understanding of it to be able to resolve its issues easily. Actually a colleague faced AWS EC2 errors and the Nginx there was not working as a reverse proxy.
  - **SETUP GUIDE**
    - Download and unzip/extract the file to your desired location
    - Open the extracted folder in *Command Prompt*, you will find *nginx.exe* there
    - type `nginx` in *Command Prompt*, or run the *nginx.exe* file
    - Open your web browser, and go to `http://localhost:80`, you will find the default page there
    - Edit the `nginx.conf` file the same folder under `conf/`, it compromises of simple and block directives
- Reverse Proxying using Nginx is to have a Rate Limiting and a Load Balancer that takes in incoming requests and forwards those to the target URL without exposing the actual backend ports.
  ```bash
  # nginx-x.x/conf/nginx.conf
  http {
    server {
      listen       80;
      server_name  localhost;

      location / {
        proxy_pass http://localhost:3000/scrape; # forwards incoming request to this addresss
        proxy_set_header Host $host;             # preserves original Host header
      }
    }
  }
  ```