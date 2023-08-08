# first create playbook and save as nginx-playbook.yml
<pre>
---

- name: Install and start nginx
  hosts: all
  become: true

  tasks:
    - name: Install nginx
      apt:
        name: nginx
        state: present
    - name: Start nginx
      service:
        name: nginx
        state: started
~                         
</pre>

# start playbook 
  
**ansible-playbook -i inventory nginx-playbook.yml** 



![Screenshot from 2023-08-08 17-40-28](https://github.com/Manoj123-github/Ansible/assets/76830665/9460326d-c078-4411-940c-faef426458a2)



# now check on target server that nginx is installed or not

![Screenshot from 2023-08-08 17-46-15](https://github.com/Manoj123-github/Ansible/assets/76830665/bd44d24a-3243-4f06-94f7-584b252473fc)

