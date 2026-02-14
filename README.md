# Nginx + Cloudflare Website Hosting

## Overview

This project demonstrates how a website was hosted on a self-managed **Ubuntu Server** using **Nginx** as the web server and **Cloudflare** for DNS and external access.

The setup allows the website to be accessed from the internet through a domain name while the server runs locally.

---

## Features

* Nginx web server installation and configuration
* Website hosted on an Ubuntu Server
* Cloudflare DNS configuration
* External access through domain name
* Firewall configuration to allow web traffic

---

## Technologies Used

* Ubuntu Server
* Nginx
* Cloudflare DNS

---

## Basic Setup Steps

### 1. Install Nginx

```bash
sudo apt update
sudo apt install nginx -y
```

### 2. Allow Web Traffic Through Firewall

```bash
sudo ufw allow 80
sudo ufw allow 443
sudo ufw enable
```

### 3. Configure Website

* Place website files in:

```
/var/www/html
```

* Restart Nginx:

```bash
sudo systemctl restart nginx
```

### 4. Configure Cloudflare DNS

* Add your domain to Cloudflare
* Create an **A record** pointing to your public IP address
* Enable the proxy if desired

---

## Result

Users can access the hosted website using the domain name managed through Cloudflare, while the content is served from the local Ubuntu server via Nginx.

---

## Purpose

This project was completed as part of a hands-on system administration practice focused on:

* Web server deployment
* DNS configuration
* Self-hosting concepts

---

## Author

**John Apomah Elike**
IT Student – Ghana Communication Technology University
Aspiring System Administrator | Cybersecurity | Cloud Computing
