**Project Summary**

We need to integrate Github with jenkins, jenkins-server with Ansible-server and ansible-server with web-server. 

**1**. Then developer will write source code and commit and then push to github.

**2**. When pushed to Github, Jenkins will start the job-compiling and building and jenkins will transfer the output file to ansible server. 

**3**. When ansible server receives file, jenkins will trigger playbook mentioned in ansible server. Playbook mentions to deploy the software on web server. 

**4**. In future, any changes done by developer and pushed to Github, job will start running again and new version of software will be deployed.

We need 4 ec2 instance for 4 servers, Github server is provided by github, so we need to create for ansible, jenkins, web server, developer ie 4 ec2 instances.
