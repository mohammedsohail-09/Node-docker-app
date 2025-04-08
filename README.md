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

![Screenshot 2025-04-08 234132](https://github.com/user-attachments/assets/95e8f7d5-0824-46f1-b2db-eec2f0289de0)

![Screenshot 2025-04-08 234929](https://github.com/user-attachments/assets/9c0211c6-a176-42ca-a437-56e48375738e)

🚀 Run Docker Container

docker run -p 3000:3000 my-node-app

Then open: http://localhost:3000

🧪 Sample Output

Hello from Node!

![Screenshot 2025-04-08 234951](https://github.com/user-attachments/assets/c00cb525-d9e6-4fc1-bb8c-d51e2a207380)

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

![Screenshot 2025-04-08 204332](https://github.com/user-attachments/assets/80a47027-fe13-437f-9917-ce7b600371e5)

![Screenshot 2025-04-08 204430](https://github.com/user-attachments/assets/f2a8b8e8-ffb5-44cc-a175-4a92b9ac0ec9)

![Screenshot 2025-04-08 204528](https://github.com/user-attachments/assets/fcccf586-1ed8-4bfb-b4b0-c44e2023d246)

![Screenshot 2025-04-08 204546](https://github.com/user-attachments/assets/10697ce3-2d77-459e-9f13-0d938ed206bb)

![Screenshot 2025-04-08 205001](https://github.com/user-attachments/assets/af52a062-6de4-4eb4-9145-475f3b7cf57b)

![Screenshot 2025-04-08 205020](https://github.com/user-attachments/assets/6e12b7a7-6ed3-45e2-b292-ff608c8ef2bf)

![Screenshot 2025-04-08 221925](https://github.com/user-attachments/assets/f942f444-14a4-4f77-bf46-4b03b77355d9)

![Screenshot 2025-04-08 221934](https://github.com/user-attachments/assets/6b259182-4e5d-446c-af10-0c4603aa2834)

![Screenshot 2025-04-08 221948](https://github.com/user-attachments/assets/540b9384-ac40-4a1c-bc55-ca6685c491a3)

![Screenshot 2025-04-08 221957](https://github.com/user-attachments/assets/14ebb88f-feed-4fb8-9f1a-f2ee37fa0b8e)

![Screenshot 2025-04-08 221957](https://github.com/user-attachments/assets/a74e8f01-862d-45d6-9388-8f29be4a698f)

👨‍💻 Author
Mohammed Sohail
Connect with me on LinkedIn
