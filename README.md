# Jenkins Custom Docker Image – Freestyle Job 🚀

##  Project Title
**Build and Deploy a Custom Docker Image using Jenkins Freestyle Project**

---

##  Project Objective
This project demonstrates how to use **Jenkins Freestyle Job** to:
- Pull source code from GitHub
- Build a **custom Docker image**
- Deploy (run) the Docker cont

---
##  Tools & Technologies Used
- Jenkins  
- Docker  
- Git & GitHub  
- Linux (Ubuntu)
---
## Step-by-Step Implementation

**Step1: Launch a Jenkins Server and inside install jenkins**
- sudo apt update 
- sudo apt upgrade -y
- udo apt install openjdk-17-jdk -y
- java -version
- Add Jenkins Repository Key
  Add the Jenkins official GPG key.
- Add Jenkins Repository  
- sudo apt update
- sudo apt install jenkins -y
- sudo systemctl start jenkins

![](/Images/Jenkins%20Server.png)

---

**Step2: Set the Jenkis IP**

-  /var/www/jenkins/ 
- nano jenkins.model.JenkinsLocationConfiguration.xml file

![](/Images/SSH%20and%20cmds.png)

---

**Step3: Create directory**
- /nodeapp
- Inside /nodeapp
- package.json,app.js,Dockerfile

**Step4: Install docker**
- sudo apt install docker.io -y

**Step5: Create a Github Repoitory**
- Copy the repository link

![](/Images/Gihub%20repo.png)

---

**Step6: Login Jenkins On browser**
- JenkinsIP:8080

![](/Images/Login%20to%20browser.png)

---

**Step7: In Jenkins Create a New Item**
- name
- Description= To build custom image
- Trigger= Github hook trigger
- Build Step->Execute shell

![](/Images/Jemkis%20Item%201.png)
![](/Images/2.png)
![](/Images/3.png)
![](/Images/4.png)

---

**Step8: Add webhook in your github**
- Fill yopur current jenkins IP Address

![](/Images/Add%20webhook.png)


---

**Step9: Push the file on github through commands**

![](/Images/cmds.png)

![](/Images/adds%20file%20on%20gihub.png)

---

**Step10: Console Output**

![](/Images/Console%20output.png)

![](/Images/output%20success.png)

## Conclusion:
Jenkins was installed on the server and integrated with Docker to build and run a custom Docker image automatically. This project helped in understanding basic CI automation using Jenkins and Docker.