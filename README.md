# Node.js CI/CD with GitHub Actions & AWS EC2 🚀

This project demonstrates a complete CI/CD pipeline using **GitHub Actions** for a **Node.js Express app**, with automatic deployment to an **AWS EC2 instance** on every push to the `main` branch.

## 🔧 Tech Stack
- Node.js (Express.js)
- GitHub Actions (CI/CD)
- AWS EC2 (Ubuntu Free Tier)
- PM2 for process management

## 📦 Features
- Auto-deploy on every push to `main`
- SSH-based secure deployment to EC2
- Uses PM2 to keep the app running
- Easily extensible for testing, linting, Docker, and more

## 📁 Folder Structure

📦nodejs-github-actions-cicd
┣ 📂.github
┃ ┗ 📂workflows
┃ ┗ 📜deploy.yml
┣ 📜index.js
┣ 📜package.json


## 🔐 Secrets Needed
Go to your GitHub repo → Settings → Secrets → Actions → Add:
- `EC2_SSH_KEY`: Your EC2 private key (from .pem file)

## 🚀 How It Works
1. Code is pushed to GitHub
2. GitHub Actions workflow is triggered
3. The workflow:
   - Connects to EC2 via SSH
   - Pulls latest code
   - Installs dependencies
   - Restarts the app with PM2

---

## 🧠 Author
Maintained by [Jenes Devganiya](https://github.com/Jenesh18)

