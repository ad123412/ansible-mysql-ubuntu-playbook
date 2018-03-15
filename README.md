# ansible-mysql-ubuntu-playbook


run the playbook
=============================
ansible-playbook -i inventories/dev --vault-password-file=vault_password.txt site.yml


create encrypted mysql root password (mysql_root_password) using valult
=======================================================================

run the command inside (roles/mysql/vars) ==> "ansible-vault create main.yml"
then enter the password 'mysql_root_password: <password>' in the above file opened in default editor
save it and clode it. it will encrypt automatically.
