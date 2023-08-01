# AltSchool Cloud-Engineering Exercises

## [Exercise]() 1
### Task: 
* Setup Ubuntu 20.04 LTS on your local machine using Vagrant
### Instruction: 
- [ ] Customize your Vagrant file as necessary with private_network set to DHCP.
- [ ] Once the machine is up, run ifconfig and share the output in your submission along with your Vagrant file in a folder for this exercise.

## [Exercise]() 2
### Task: 
* Research online for 10 more Linux commands aside from the ones already mentioned in this module. Submit using your AltSchool-cloud-exercises project, explaining what each command is used for with examples of how to use each and example screenshots of using each of them.

### Instruction:
- [ ] Submit your work in a folder for this exercise in your AltSchool-cloud-exercises project. You will need to learn how to embed images in markdown files.

## [Exercise]() 3
### Task:
* Create 3 groups – admin, support & engineering and add the admin group to sudoers. 
* Create a user in each of the groups. 
* Generate SSH keys for the user in the admin group.
### Instruction:
- [ ] Submit the contents of /etc/passwd, /etc/group, /etc/sudoers

## [Exercise]() 4
### Task: 
* Install PHP 7.4 on your local Linux machine using the ppa:ondrej/php package repo.
### Instruction:
- [ ] Learn how to use the add-apt-repository command
- [ ] Submit the content of /etc/apt/sources.list and the output of php -v command

## [Exercise]() 5
### Task: 
* You already have a GitHub account, also set up a GitLab account if you don’t have one already.
* You already have an AltSchool-cloud-exercises project, clone the project to your local system.
* Setup your name and email in Git’s global config.
### Instruction:
Submit the output of:
- [ ] git config -l
- [ ] git remote -v
- [ ] git log

## [Exercise]() 6
### Task: 
* Review the CIS benchmark for Ubuntu, and try to implement at least 10 of the recommendations that we made within the benchmark.

### Instruction:
  -  N/A

## [Exercise]() 7

### Task:

* Create a bash script to run every hour, saving system memory (RAM) usage to a specified file, and at midnight it sends the content of the file to a specified email address, then starts over for the new day.

### Instruction:

- [ ] Submit the content of your script, cronjob, and a sample of the email sent, all in the folder for this exercise.

## [Exercise]() 8

### Task:
* Create an Ansible Playbook to set up a server with Apache
* The server should be set to the Africa/Lagos Timezone
* Host an index.php file with the following content, as the main file on the server:
```php
<?php
date_default_timezone_set('Africa/Lagos');
echo date("F d, Y h:i:s A e", time());
?>
```

### Instruction:
- [ ] Submit the Ansible playbook, the output of `systemctl status apache2` after deploying the playbook, and a screenshot of the rendered page

## [Exercise]() 9

### Task:

> 193.16.20.35/29

* What is the Network IP, number of hosts, range of IP addresses, and broadcast IP from this subnet?

### Instruction: 
- [ ] Submit all your answers as a markdown file in the folder for this exercise.


# MINI PROJECT ([Exercise]() 10)

We will be deploying a real-life application:
- Demo Project: https://github.com/f1amy/laravel-realworld-example-app
- Setup Debian 11 on a virtual machine instance with a cloud provider or as instructed
- Setup Apache with every dependency the application needs to run
- Don't use Laravel Sail or Docker as suggested in the project README file, simply clone the project with Git and deploy with Apache
- Setup MySQL with credentials and a database for your application to use
- Configure a subdomain if you have a domain name to point the VM instance or speak to an instructor for further guide
- You have completed the project if you are able to view the application according to the specifications in the project from your Host browser

# EXAM PROJECT ([Exercise]() 11)
## Question
​
- You are required to deploy the same Laravel application from your mini project.
- This time, the entire deployment steps including installation of packages and dependencies, configuring your Apache webserver, etc, will be defined in an Ansible playbook and deployed to at least one Ansible slave.
- You should also write a bash script that would install and set up Postgresql.
- This bash script would be run on your Ansible slaves using an Ansible playbook.

## Requirements
​
- We should be able to access your deployment using a domain name of your choice(not an IP address).
- We should be able to test all the endpoints without errors.
- Your base URL may or may not display the default Laravel page.
- These must be done on virtual machines on any cloud provider of your choice(any Linux distro of your choice).
- Your application must be encrypted with TLS/SSL.
- You may or may not define a logical network on the cloud, but extra efforts would be rewarded.

## Submission
​
- Push your code to GitHub 
- Share your GitHub link on the shared document.
- Share your cloud credentials.

### Note: 
You can create IAM users for your instructors with the least privilege but enough to view your instances, the firewall rules set on your instance, and any logical network if set. If this would require sharing your ssh keys, please do so privately. 
​
​
​
## Helpful links
​
- https://medium.com/@melihovv/zero-time-deploy-of-laravel-project-with-ansible-3235816676bb

- https://www.cherryservers.com/blog/how-to-install-and-setup-postgresql-server-on-ubuntu-20-04
​
- https://dev.to/sureshramani/how-to-deploy-laravel-project-with-apache-on-ubuntu-36p3

## Best of luck!
