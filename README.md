# Instal_jenkins_and_run_ansible_test
This task was for how to running and install jenkins (ansible as the test) in to Ubuntu 18++


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
- 
- 
- 
- 
- 

Install Ansible

