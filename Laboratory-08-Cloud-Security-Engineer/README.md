# Mission 8 — The Cloud Security Engineer

## Mission Overview

This mission demonstrates how to secure a Linux web server using the Uncomplicated Firewall (UFW). The activity deploys an Nginx container, checks application access, applies a default deny incoming policy, and selectively allows required traffic.

## Objectives

- Understand the Principle of Least Privilege and attack surface.
- Deploy an Nginx web application on port 8080.
- Audit firewall status and network access.
- Configure UFW with a default deny incoming policy.
- Allow SSH and the required application port.
- Document firewall configuration and security practices.

## Commands Executed

- `docker run -d --name secure-web-app -p 8080:80 nginx`
- `curl -s http://localhost:8080 | head -n 5`
- `sudo ufw allow ssh`
- `sudo ufw default deny incoming`
- `sudo ufw default allow outgoing`
- `sudo ufw enable`
- `sudo ufw status verbose`
- `sudo ufw allow 8080/tcp`
- `sudo ufw status numbered`

## Skills Learned

This mission developed practical skills in Docker deployment, Linux firewall configuration, network port management, security auditing, Markdown documentation, and GitHub portfolio maintenance.


