# ansible-playbooks

## sshでの接続確認
ssh-keygen -R 160.xxx.xxx.xxx
ssh root@160.xxx.xxx.xxx

## CentOS7での初期設定用
cd /ansible-playbooks/centos7
ansible-playbook -i hosts -u root centos7_init.yml -k --check
ansible-playbook -i hosts -u root centos7_init.yml -k

## sshでの接続確認
ssh user@160.xxx.xxx.xxx -p 10022

## CentOS7でhttpの設定
ansible-playbook -i hosts -s -u user http.yml --check
ansible-playbook -i hosts -s -u user http.yml

## CentOS7でftpの設定
ansible-playbook -i hosts -s -u user ftp.yml --check
ansible-playbook -i hosts -s -u user ftp.yml

## CentOS7でphpの設定
ansible-playbook -i hosts -s -u user php.yml --check
ansible-playbook -i hosts -s -u user php.yml

## CentOS7でmariadbの設定
ansible-playbook -i hosts -s -u user mariadb.yml --check
ansible-playbook -i hosts -s -u user mariadb.yml

## CentOS7でwp-cliの設定
ansible-playbook -i hosts -s -u user wp-cli.yml --check
ansible-playbook -i hosts -s -u user wp-cli.yml
