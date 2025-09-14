⚙️ Setup Steps
=

### 1. Prepare Your Application
- Add your application code to this repository.
- Ensure dependencies are listed (requirements.txt, package.json, or build file depending on language).

### 2. Create Elastic Beanstalk Environment
=
-In the **AWS Management Console**, go to **Elastic Beanstalk**.
- Create a new application and environment (Web-deploy-env).
- Select the correct platform (Node.js, Python, Java, etc.).
- Note the **Web-deploy** and **Web-deploy-env**.
  
![image_alt](https://github.com/meghapawar177-droid/-Deploy-Web-Application-from-GitHub-to-AWS-Elastic-Beanstalk-using-CodePipeline/blob/ea2583554550dba9fd45f5ee3e8c7d385edf7f13/new/eb1.png)
![image_alt](https://github.com/meghapawar177-droid/-Deploy-Web-Application-from-GitHub-to-AWS-Elastic-Beanstalk-using-CodePipeline/blob/62645bb17be2788a7522e8285efea0878183b833/new/f_eb.png)
---

### 3. Configure IAM Role
=
 - Open **IAM Role ** in the console.
 - Create Role (Elastic Benstalk Role).
 - Add policies in the Role.
 ![image_alt](https://github.com/meghapawar177-droid/-Deploy-Web-Application-from-GitHub-to-AWS-Elastic-Beanstalk-using-CodePipeline/blob/d5e9507b47cb0117cd3c3011a17259413d0d1ffc/new/Role.png)

### 4. Configure CodePipeline
=
- Open **AWS CodePipeline** in the console.
- Create connection to github.
- Create a new pipeline and give it a name.
- **Source Stage**: Choose *GitHub* and connect to this repository.
- **Build Stage (Optional)**: You can add a build step with AWS CodeBuild if your app needs compiling or testing.
- **Deploy Stage**: Choose *Elastic Beanstalk* and select your application and environment.
- Save and create the pipeline.
![img_alt](https://github.com/meghapawar177-droid/-Deploy-Web-Application-from-GitHub-to-AWS-Elastic-Beanstalk-using-CodePipeline/blob/8a11b94f3913fd67fe1b96567762c4dcc8edf14c/new/pipeline.png)

### 5. Check final output
=
Refresh the page of Elastic Beanstalk.
![alt text](https://github.com/meghapawar177-droid/-Deploy-Web-Application-from-GitHub-to-AWS-Elastic-Beanstalk-using-CodePipeline/blob/0db9db8353d16e917af26d3b6a3243056d7ca88e/new/final%20output.png)
