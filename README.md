**## DevOps Task Stage 0 - NGINX Configuration**

## Project Overview
This project demonstrates the deployment of a static website using a cloud platform and a web server. It encompasses essential DevOps practices like server configuration (with nginx) and automation without going too deep into other technical areas. The goal is to deploy a static website that is accessible via a public IP address or domain name.

## About site
The site is a simple static website that displays a welcome message. It is a practice project and part of an introductory/test task for the HNG intership program.

## Technologies Used
For the purpose of this project the following technologies were used:
static website: written in HTML and styled with CSS and JavaScript
Cloud Platform: Google Cloude Platform
Web Server: configured and deployed with NGINX 

## Project Structure

**
├── index.html
├── styles.css
├── script.js
├── server_config
│   ├── nginx.conf
└── README.md
**
## Setup Guide

### Prerequisites
- A fresh Ubuntu server (18.04 or later)
- SSH access to the server
- Basic knowledge of terminal commands

### Step-by-Step Guide

1. **Update the Server**
    ```bash
    sudo apt update
    sudo apt upgrade -y
    ```

2. **Install NGINX**
    ```bash
    sudo apt install nginx -y
    ```

3. **Start and Enable NGINX**
    ```bash
    sudo systemctl start nginx
    sudo systemctl enable nginx
    ```

4. **Verify NGINX Installation**
    Open your web browser and navigate to `http://<your-server-ip>/`. You should see your custom welcome message.

### Troubleshooting
- If NGINX is not running, check the status with:
    ```bash
    sudo systemctl status nginx
    ```
- Check NGINX error logs for more details:
    ```bash
    sudo tail -f /var/log/nginx/error.log
    ```

### Reference
- [DevOps Engineers](https://hng.tech/hire/devops-engineers)
- [Google Cloud Engineers](https://hng.tech/hire/google-cloud-engineers)

## License
This project is part of the HNG Internship program. To know more follow the link https://hng.tech/
©2024 shamsaine...
