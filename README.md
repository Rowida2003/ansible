ansible tasks 
folder task1 ---- Initial Ansible Configuration and Ad-Hoc Execution
steps:
Install Ansible Automation Platform on the control node.
Configure Ansible on the control node for management tasks.
Generate a new SSH key pair on the control node.
Copy the public key from the control node to the managed node to enable passwordless SSH access.
Create an inventory file listing the managed node(s) for Ansible to manage.
Run an ad-hoc command from the control node to check disk space on the managed node and verify connectivity.

folder roles ---- Structured Configuration Management with Ansible Roles
steps:
Create an Ansible role for Docker installation and configuration.
Create an Ansible role for Kubernetes CLI (kubectl) installation and setup.
Create an Ansible role for Jenkins installation and basic configuration.
Write an Ansible playbook that includes and runs all the created roles.
Execute the playbook from the control node to apply configurations on the managed node(s).
Verify that Docker, kubectl, and Jenkins are installed and functioning correctly on the managed node.

folder nginx ---- Automated Web Server Configuration Using Ansible Playbooks
steps:
Install Nginx on the managed node.
Ensure the Nginx service is started and enabled to run at boot.
Replace the default Nginx web page with a custom page.
Set correct permissions for the web page files.
Verify Nginx is running properly on the managed node.
Test the web page to confirm the custom content is displayed.

folder ansible-mysql ---- Securing Sensitive Data with Ansible Vault
steps:
nstall MySQL on the managed node.
Create a database named iVolve.
Create a database user and grant all privileges on the iVolve database.
Encrypt sensitive information, such as the database user password, using Ansible Vault.
Write an Ansible playbook that applies the above tasks securely.
Run the playbook from the control node to configure the managed node.
Validate the database by connecting with the created user and listing the databases to ensure proper setup.
