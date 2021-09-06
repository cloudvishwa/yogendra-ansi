
# Flow of the Ansible script.



## 1. Setup Jenkins 
## ansible-playbook -i inventory add-cred.yml jenkins.yml


## 2. Add credentials
## ansible-playbook -i inventory add-cred.yml -e "key_name=ansible.pem" -e "cred_id_name=slave_cred" -e "cred_usr=centos" -e "jen_usr=jenkins" -e "jen_pwd=Reset123"

## 3. Add Salve Node
## ansible-playbook -i inventory Jenkins_slave.yml -e "Hostid=192.168.68.211" -e "Cred_Id=slave-local-id" -e "slavename=java-s1" -e  "path_list=/root/project1" -e "execu=1" -e "label_01=java" -e "jen_usr=jenkins" -e "jen_pwd=Reset123"
