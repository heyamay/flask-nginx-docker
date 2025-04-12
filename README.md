# 🚀 Domain-Integrated Flask App Deployment using Docker, Nginx, Route 53, ACM, and GitHub Actions

![Architecture Diagram](https://github.com/heyamay/flask-nginx-docker/blob/master/banner.png)
This project demonstrates the deployment of a Flask application using Docker and Nginx, integrated with AWS services such as Route 53 for domain management and ACM for SSL certification. The deployment process is automated using GitHub Actions, ensuring continuous integration and delivery.

---

## 🧰 Tech Stack

- **Flask** – Python web framework for building the application.
- **Docker** – Containerization platform to package the application.
- **Nginx** – Web server acting as a reverse proxy.
- **AWS Route 53** – Domain name system (DNS) web service.
- **AWS Certificate Manager (ACM)** – Provisioning and managing SSL/TLS certificates.
- **GitHub Actions** – Automating the build and deployment pipeline.

---

## 📁 Project Structure

```bash
├── app/
│   ├── app.py
├── nginx/
│   └── default.conf
├── .github/
│   └── workflows/
│       └── deploy.yml
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md
```
## 🛠️ How It Works

1. **Dockerize** the Flask app with `Dockerfile`
2. Use **Nginx** for reverse proxy and forwarding HTTPS traffic
3. Point custom domain using **Route 53**
4. Configure **SSL Certificate** using ACM for HTTPS
5. Automate deployment on every `push` to `master` via **GitHub Actions**
6. Pull and run latest image on EC2 using **Docker**

## 🌐 Domain & SSL
- Route 53: Set A Record → EC2 Public IP

- ACM: Request & validate SSL → Attach to Load Balancer or manually configure in Nginx

- Nginx Config: Update reverse proxy to listen on 443 and serve Flask via Docker container

## ✅ Result
- Auto-deploy Flask app on each push to main

- HTTPS-secured app with domain access via Route 53

- Fully containerized and production-ready setup using GitHub Actions

Feel free to reach out on LinkedIn - https://www.linkedin.com/in/heyamay/ if you're trying a similar project or want to collaborate!

# Resume

- 1. Automated CI/CD pipeline using GitHub Actions, reducing deployment time by 90% for Flask app hosted on AWS EC2 with Docker & Nginx.

- 2. Deployed scalable web app using Docker Compose, AWS ALB, and Nginx reverse proxy, handling traffic via SSL (ACM) and custom domain integration.

- 3. Managed full-stack deployment with Route 53 domain routing, ACM for HTTPS, and secure SSH-based deployment scripts via GitHub-hosted workflows.
