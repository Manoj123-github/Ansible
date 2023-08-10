# Create the role structure:

Navigate to your Ansible project directory and use the following command to create the basic structure of the role:

**ansible-galaxy init nginx_role**

This will create a directory named nginx_role with the required subdirectories and files.

# Edit the tasks/main.yml file:

Inside the nginx_role directory, go to tasks/main.yml and edit it to include the tasks for installing Nginx. Here's an example content:

<pre>
---
# tasks file for nginx_role

- name: Install Nginx
  apt:
    name: nginx
    state: latest
  become: true

</pre>

This task uses the apt module to install Nginx on the remote server.

# Use the role in a playbook:

Create a playbook that uses the nginx_role you've just created. Let's call this playbook nginx_install.yml:

<pre>
---
- name: Install Nginx on remote servers
  hosts: localhost
  become: true

  roles:
    - nginx_role
</pre>

In this playbook, replace web_servers with the group or hostname of the remote servers where you want to install Nginx.

# Run the playbook:

Run the playbook using the following command:

**ansible-playbook nginx_install.yml**

![image](https://github.com/Manoj123-github/Ansible/assets/76830665/602b97a8-b7de-4516-9da7-e6ff7a703f0b)

