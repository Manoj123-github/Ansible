# add host name and private key in inventory as below
<pre>
ubuntu@ip-172-31-21-208:~/ansible$ cat inventory 
ec2-54-162-160-121.compute-1.amazonaws.com ansible_ssh_private_key_file=/home/ubuntu/ansible/keys/ansible.pem
ec2-35-173-124-104.compute-1.amazonaws.com ansible_ssh_private_key_file=/home/ubuntu/ansible/keys/ansible.pem

</pre>

# now run playbook as usual 

<pre>
---
- name: Update and Upgrade APT Packages
  hosts: all
  become: true

  tasks:
    - name: Update APT package cache
      apt:
        update_cache: yes


    - name: Upgrade APT packages
      apt:
        upgrade: yes
~                                                                                                                                                
  
</pre>

Now run playbook

**ansible-playbook -i inventory instll-playbook.yml**

![image](https://github.com/Manoj123-github/Ansible/assets/76830665/4da15249-ffbb-4ec4-8074-56afb0086eab)
