# Instal_jenkins_and_run_ansible_test
This task was for how to running and install jenkins (ansible as the test) in to Ubuntu 18++


++++
=====JENKINS=====
++++
Step 1 install Jenkins:
- sudo apt-get update
- sudo apt-get install openjdk-8-jdk
- wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
- sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
- sudo apt-get update
- sudo apt-get install jenkins
- sudo apt install git
on this steps we success to install Jenkins now we can check service for jenkins to see it running
- service jenkins status

Now we ready to access the jenkins "localhost:8080/<your ip>:8080" after login you can follow the install procedure inside the jenkins !
Link source: https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/jenkins-ubuntu-20-install-git-jdk-java-ci-cd 
Tools that I install to Jekins: 
- Active Choices Plug-in
- Active Directory plugin
- AnsiColor
- Ant Plugin
- Build Name and Description Setter
- bouncycastle API Plugin
- Build Timeout Version 
- Command Agent Launcher Plugin Version 
- Create Job Advanced
- Downstream-Ext
- Dynamic Extended Choice Parameter Plug-In
- Editable Choice Plugin
- Email Extension Template Plugin
- Extended Choice Parameter Plug-In
- Extended Read Permission Plugin
- Extended Security Settings Plugin
- GitHub Branch Source Plugin
- Gradle Plugin
- Green Balls
- LDAP Plugin
- LIFX notifier - smart lightbulbs build indicator
- Logging Plugin
- Maven Artifact ChoiceListProvider (Nexus)
- PAM Authentication plugin Version 
- Persistent Parameter Plugin
- Pipeline
- Pipeline timeline
- Pipeline: GitHub Groovy Libraries
- Pipeline: Stage View Plugin
- Remote Terminal Access plugin
- SSH Agent Plugin
- SSH Build Agents plugin
- SSH Pipeline Steps
- SSH plugin
- Terraform Plugin
- Text File Operations
- Timestamper
- Workspace Cleanup Plugin Version 

Now all setup to jenkins, one more step to let Jenkins Run the service using sudo: 
- sudo visudo
  - add the code in the bottom for give permission jekins
    - jenkins ALL=(ALL) NOPASSWD: ALL
  - in the same file add collor code to allow ansible show the log with the color in jenkins
    - Defaults        env_reset
    - Defaults        env_keep += "ANSIBLE_FORCE_COLOR"

++++
=====ANSIBLE=====
++++
Install Ansible

