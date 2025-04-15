# 🚀 Node.js Dockerized App

Welcome to the **Node.js Docker App**! This is a simple Express.js application containerized using Docker. It serves as a beginner-friendly guide to building, running, and deploying Node apps with Docker — ideal for DevOps learning or full-stack practice!

---

## 🛠️ Tech Stack

- **Node.js** (v18/20)
- **Express.js**
- **Docker**
- **Jenkins** 

---

## 📁 Project Structure


---

## ⚙️ Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/mohammedsohail-09/node-docker-app.git
cd node-docker-app

### 2️⃣ Install Dependencies

npm install

### 3️⃣ Run Locally

node app.js

Open your browser at: http://localhost:3000
You should see: "Hello from Node!"

🐳 Docker Instructions
📦 Build Docker Image

docker build -t my-node-app .

🚀 Run Docker Container

docker run -p 3000:3000 my-node-app

Then open: http://localhost:3000

🧪 Sample Output

Hello from Node!

✅ CI/CD with Jenkins 
If you're using Jenkins:

Ensure Jenkins has Docker privileges.

Create a Pipeline project.

Use the Jenkinsfile

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Docker image...'
                sh 'docker build -t my-node-app .'
            }
        }
        stage('Run') {
            steps {
                echo 'Running container...'
                sh 'docker run -d -p 3000:3000 my-node-app'
            }
        }
    }
}

👨‍💻 Author
Mohammed Sohail
