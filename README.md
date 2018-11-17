# Ansible Playbook with setup web server using EasyEngine as basis. 

More information about EasyEngine can be found at https://easyengine.io/

OS requirements Ubuntu 14+

# Followig ansible variables can/should be used during executing
aws_access_key_id - AWS access key for backup user \
aws_secret_access_key - AWS secret key for backup user \
ee_name - Name which will be used during EE setup \
ee_email - email address which will be used for EE setup and Let's Encrypt \

# Example of executing
```
ansible-playbook  -i <IP_OF_SERVER> -u root ee-ansible.yaml --extra-vars "aws_access_key_id=XXXXXXXXXXXX aws_secret_access_key=YYYYYYYYYYYYYYY ee_name=Test ee_email=ansible@ansible.com"
```
