# CI/CD Pipeline for Dockerized Web Application 🚀

## 📌 Project Overview
This project demonstrates the implementation of a **CI/CD (Continuous Integration and Continuous Deployment) pipeline** to automatically deploy a **Dockerized web application** on **AWS EC2** using **GitHub Actions**.  
Whenever code is pushed to the GitHub repository, the pipeline automatically builds and deploys the application without manual intervention.

---

## 🎯 Objectives
- Automate application deployment using CI/CD
- Containerize a web application using Docker
- Deploy the application on AWS EC2
- Reduce manual errors and deployment time
- Follow real-world DevOps practices

---

## 🛠️ Technology Stack
- **Cloud Platform:** AWS (EC2, VPC)
- **Version Control:** Git, GitHub
- **CI/CD Tool:** GitHub Actions
- **Containerization:** Docker
- **Web Server:** Nginx
- **OS:** Ubuntu Linux
- **Languages:** HTML, CSS, JavaScript
- **Configuration:** YAML, Shell Scripting

---

## 🧱 Project Architecture

Developer → GitHub → GitHub Actions → EC2 → Docker Container → Web Application

---

## 🔄 CI/CD Workflow
1. Developer pushes code to GitHub
2. GitHub Actions pipeline is triggered
3. Pipeline connects to EC2 using SSH
4. Docker image is built on EC2
5. Old container is stopped and removed
6. New container is deployed automatically
7. Application becomes live on EC2

---

## 📂 Project Structure

---

## 🔄 CI/CD Workflow
1. Developer pushes code to GitHub
2. GitHub Actions pipeline is triggered
3. Pipeline connects to EC2 using SSH
4. Docker image is built on EC2
5. Old container is stopped and removed
6. New container is deployed automatically
7. Application becomes live on EC2

---

## 📂 Project Structure
CI-CD Pipeline Project/
└── Source Code/
├── index.html
├── style.css
├── script.js
├── images/
└── Dockerfile

---

## 🐳 Dockerfile
```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80

⚙️ GitHub Actions Workflow

The workflow is triggered on every push to the main branch and handles both build and deployment.

🔐 GitHub Secrets Used

To enable secure deployment, the following secrets are added in GitHub:

EC2_HOST – EC2 Public IP

EC2_USER – EC2 Username (ubuntu)

EC2_KEY – SSH Private Key (.pem file)

🚀 Deployment

After successful pipeline execution, the application can be accessed using:

http://<EC2_PUBLIC_IP>

Features

Fully automated CI/CD pipeline

Dockerized application deployment

Secure SSH-based deployment

Consistent and reliable builds

Easy to scale and extend

🔮 Future Enhancements

Use AWS ECR for Docker image storage

Deploy using ECS or Kubernetes

Add load balancer and auto-scaling

Implement rollback mechanism

Enable monitoring with CloudWatch

Add HTTPS using Route 53 and SSL


📖 Conclusion

This project showcases how DevOps tools like GitHub Actions and Docker can be integrated with AWS EC2 to build a reliable and automated CI/CD pipeline, reflecting real-world deployment practices.

👤 Author

Naren M K


📝 License

This project is for educational and learning purposes.


---

### ✅ What you should do next
1. Save this as **`README.md`**
2. Push to GitHub:
```bash
git add README.md
git commit -m "Add project README"
git push origin main