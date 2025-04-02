# Flask DevOps CI/CD Project

This project demonstrates containerizing a Flask application with Docker and implementing CI/CD using GitHub Actions.

## 🚀 Features

- ✅ **Flask Web App** – A simple app returning "Hello DevOps!"
- ✅ Flask DevOps CI– Uses a multi-stage build for optimized image size
- ✅ps CI/CD Project

Th– Automatically builds and pushes to Docker Hub on push & PR
- ✅Project

This projec– Runs tests & deploys the app

## 📂 Project Structure

flask-devops/
│── .github/workflows/ci-cd.yml  # CI/CD workflow
│── app.py                        # Flask application
│── requirements.txt               # Dependencies
│── Dockerfile                     # Multi-stage build
│── .dockerignore                  # Exclude files from Docker
│── .gitignore                     # Exclude files from Git
│── README.md                      # Documentation

## 🔧 Setup & Run Locally

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/flask-devops.git
cd flask-devops

2️⃣ Build & Run Docker Container

docker build -t flask-devops .
docker run -p 5000:5000 flask-devops

👉 Open http://localhost:5000/ in your browser.

🚀 CI/CD Pipeline (GitHub Actions)

 • ✅ On Push – Builds & pushes Docker image to Docker Hub
 • ✅ On Pull Request – Runs build tests (but does not push)

GitHub Secrets Required

 • DOCKERHUB_USERNAME – Your Docker Hub username
 • DOCKERHUB_PASSWORD – Your Docker Hub password
