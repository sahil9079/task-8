# 🧩 Task 8: Run a Simple Java Maven Build Job in Jenkins

## 🎯 Objective
<img width="1920" height="1080" alt="Screenshot (473)" src="https://github.com/user-attachments/assets/a66f793b-c1df-475e-b63a-6068f57ea28e" />

Use **Jenkins** and **Maven** to build a simple Java application — your first step into CI/CD automation.


<img width="1920" height="1080" alt="Screenshot (475)" src="https://github.com/user-attachments/assets/0db20b22-ee5a-4d8c-8db2-a6ea1d0ee4b9" />


<img width="1920" height="1080" alt="Screenshot (479)" src="https://github.com/user-attachments/assets/107cc1c5-492e-4dc3-9dbd-aebb3c195c68" />


<img width="1920" height="1080" alt="Screenshot (481)" src="https://github.com/user-attachments/assets/850d99f8-cbd3-42c0-936b-31682aa9cb1a" />


<img width="1920" height="1080" alt="Screenshot (483)" src="https://github.com/user-attachments/assets/fcb5c15e-a4ee-4008-8db4-fe73144c933d" />


---

## 🛠 Tools Used
- Jenkins (via Docker)
- Java JDK 8/11  
- Maven  
- Git  

---

## 📂 Project Structure
hello-java-maven/
├── pom.xml
└── src/main/java/HelloWorld.java

csharp
Copy code

### HelloWorld.java
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, Jenkins + Maven!");
    }
}
⚙️ Jenkins Setup
Run Jenkins:
<img width="1920" height="1080" alt="Screenshot (479)" src="https://github.com/user-attachments/assets/2eefbd88-6153-4996-ae7f-808fcf5bbb42" />

bash
Copy code
docker run -d --name jenkins -p 8080:8080 jenkins/jenkins:lts
Go to Manage Jenkins → Global Tool Configuration
Add Maven (e.g., Maven 3.8.6).

🚀 Job Configuration
Source Code Management: Git → https://github.com/sahil9079/task-8.git
<img width="1920" height="1080" alt="Screenshot (484)" src="https://github.com/user-attachments/assets/590cd282-e5a9-4214-865d-e72d4b0118b2" />

Branch: */main

Build Step: Invoke top-level Maven targets → clean package

Post-build Action (optional): Archive target/*.jar

✅ Build Result
Open Console Output → You should see:
<img width="1920" height="1080" alt="Screenshot (482)" src="https://github.com/user-attachments/assets/43242b9c-f5bc-4f09-b822-ac7cc0f8818f" />

csharp
Copy code
[INFO] BUILD SUCCESS
📸 Screenshot of successful build below:

<img width="1920" height="1080" alt="Screenshot (483)" src="https://github.com/user-attachments/assets/0019196f-b1ca-4ec4-8b2b-54323d7e8361" />

👨‍💻 Author
Sahil Khan
DevOps Enthusiast | Learning CI/CD with Jenkins + Maven

yaml
Copy code

---

💡 Tip:  
Just place your screenshot in the repo (same folder as README) and name it `screenshot.png` so it displays correctly.

Would you like me to include a one-line **troubleshooting tip** section (for Maven/JDK errors) at 

---
=

