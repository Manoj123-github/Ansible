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
  
ansible-playbook -i inventory nginx-playbook.yml 



