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

![image](https://github.com/Manoj123-github/Ansible/assets/76830665/9591326f-2e76-4e20-95f8-579a398d916c)
