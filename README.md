# Project Eden
An Automated Infrastructure-as-Code development system

### Goal:
- The goal of this project is to provide an open-source system that can serve the community in Cybersecurity education, testing, development, etc.  The community wouldn't have to worry about creating repeatable infrastructure code, as this itself can be templated and produced by the project.
- This project makes sharing configurations easier for creating vulnerable and repeatable environments

### Version:
v0.0

### NOTE:
If you're reading this document, know the code will be posted shortly.  Just cleaning up prior.  Thank you for your patience, please stay tuned!

### This project can:
- Create Terraform code for AWS or Azure (GCP to come soon)
- Bridge Terraform and Ansible to create a dynamic infrastructure
- Facilitate easier sharing, production, and configuration of Ansible Role code

*\*All mentioned items are owned by their respective entities.*

### Consequently, this program makes the following much easier:
- Setting up and sharing training environments
- Standing up honeypots
- Practicing application development and testing

### Requirements to run the program:
- We'll first need to ensure we have a terminal or CMD environment (by preference, though you could also just run the gui)
- We'll also need Python3 installed
- Next, we'll need to install any required dependencies (e.g. via pip3)

### Officially running the program [from the terminal within the correct folder]:
     python3 gui.py

### How does the program work you may ask?
- The user currently supplies or modifies Ansible roles, selectable systems, selectable services, and selectable vulnerabilities
- The code in-turn uses this information to further create Terraform code, which invokes a Bash script on a remote Ansible machine in AWS/Azure
- The remote Ansible jumpbox created will create the official playbook, invoke the correct roles, and configure the other machines accordingly

### Limitations:
- This program is mostly graphical, but not entirely free from technical knowledge yet.  I have plans in motion to make it more friendly even for beginners to our field
- This program could at the same time be more friendly to automation connoisseurs who would, like me, prefer the option for terminal/CMD-line invocation; this is also in the plans

### TODO:
- Big code refactor prior to posting

### Shoutout to Redhat for their work on streamlining Ansible roles, and to Hashicorp for Terraform!
