# Ansible
Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy. Avoid writing scripts or custom code to deploy and update your applications— automate 
in a language that approaches plain English, using SSH, with no agents to install on remote systems.

Ansible is easy to deploy because it does not use any agents or custom security infrastructure.

Ansible uses playbook to describe automation jobs, and playbook uses very simple language i.e. YAML (It’s a human-readable data serialization language & is commonly used for configuration files, but could be 
used in many applications where data is being stored)which is very easy for humans to understand, read and write. Hence the advantage is that even the IT infrastructure support guys can read and understand 
the playbook and debug if needed (YAML – It is in human-readable form).

![image](https://github.com/Manoj123-github/Ansible/assets/76830665/0b6d79de-7825-420a-9e5e-7223772c3c5e)

The management node in the above picture is the controlling node (managing node) which controls the entire execution of the playbook. It’s the node from which you are running the installation. The inventory 
file provides the list of hosts where the Ansible modules needs to be run and the management node does a SSH connection and executes the small modules on the hosts machine and installs the product/software.

Beauty of Ansible is that it removes the modules once those are installed so effectively it connects to host machine , executes the instructions and if it’s successfully installed removes the code which was 
copied on the host machine which was executed.


# Installation on Ubuntu

For installing Ansible you have to configure PPA on your machine. For this, you have to run the following line of code −
<pre>
$ sudo apt-get update 
$ sudo apt-get install software-properties-common 
$ sudo apt-add-repository ppa:ansible/ansible $ sudo apt-get update 
$ sudo apt-get install ansible
</pre>

After running the above line of code, you are ready to manage remote machines through Ansible. Just run Ansible–version to check the version and just to check whether Ansible was installed properly or not.



# Some common words related to Ansible.

  **Service/Server** − A process on the machine that provides the service.

  **Machine** − A physical server, vm(virtual machine) or a container.

  **Target machine** − A machine we are about to configure with Ansible.

  **Task** − An action(run this, delete that) etc managed by Ansible.

  **Playbook** − The yml file where Ansible commands are written and yml is executed on a machine.
