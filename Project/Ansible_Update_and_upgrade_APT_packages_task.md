# Ansible - Update and upgrade APT packages task

# Write a task to update and upgrade apt packages

- name: "update and upgrade apt packages."
  become: yes
  apt:
    upgrade: yes
    update_cache: yes
