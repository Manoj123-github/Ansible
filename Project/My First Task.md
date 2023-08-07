# Write a task to create the directory ‘/tmp/new_directory’ 

# steps 1:-

first create connection between ansible server and target server using ssh-public key , to generate ssh key use ssh-keygen , and copy  public and paste in authoruzed_key in target server.
now both ansible server is able to connect target server.
    
 # step 2:-  create a inventory file and add host-ip and save it.
 
   touch inventory
   vim inventory

   # step 3:- now create ad-hoc command to create directory on the target server using below command
   
   ![image](https://github.com/Manoj123-github/Ansible/assets/76830665/fe13a9ce-474f-4b01-910b-e2f539f33145)


![image](https://github.com/Manoj123-github/Ansible/assets/76830665/e05bc5e3-c7ca-411f-9cc7-d86dc3a5160f)
