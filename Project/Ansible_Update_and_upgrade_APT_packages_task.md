# Ansible - Update and upgrade APT packages task

# Write a task to update and upgrade apt packages

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

</pre>


# output screenshot

![image](https://github.com/Manoj123-github/Ansible/assets/76830665/4b5250ca-bfb0-4be5-9ab2-6190d992633f)
