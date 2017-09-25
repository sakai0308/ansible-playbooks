# ansible-playbooks

## CentOS7での初期設定用
cd /ansible-playbooks/centos7
ansible-playbook -i hosts centos7_init.yml -k

## CentOS7でhttp,ftpの設定
ansible-playbook -i hosts http-ftp-install.yml
