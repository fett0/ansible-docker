# Docker Ansible container vyos ,how to build an image: 

sudo docker build ansible -t ansible:1.0.1
 
# Work directoy is where we have our ansible/playbooks :

 sudo docker run -v "${PWD}":/home/fett/ansible-work:ro --rm ansible:1.0.1 ansible-playbook -i hosts main.ym
