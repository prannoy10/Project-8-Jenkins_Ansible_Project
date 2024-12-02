**Project Summary**

Project Overview:

This project aims to automate the CI/CD pipeline by integrating GitHub, Jenkins, Ansible, and a web server. The process is designed to allow developers to push their code to GitHub, triggering automated build and deployment processes.

Project Flow:

1. Developer Code Commit:

The developer writes the source code and commits it to the GitHub repository.

2. Jenkins Job Trigger:

Once the code is pushed to GitHub, Jenkins automatically triggers a job to compile and build the application.

The compiled output is then transferred from Jenkins to the Ansible server.

3. Deployment via Ansible:

Upon receiving the output file, the Ansible server executes a predefined playbook triggered by Jenkins.

The playbook deploys the application to the web server.

4. Continuous Deployment:

In the future, whenever the developer makes changes and pushes the code to GitHub, the entire pipeline will be triggered again, ensuring the latest version of the software is deployed to the web server.


Infrastructure Requirements:

The system will require four EC2 instances:

1. GitHub: The repository is hosted on GitHub.

2. Jenkins: For CI/CD job execution.

3. Ansible Server: To manage deployment through playbooks.

4. Web Server: Where the application will be deployed.
