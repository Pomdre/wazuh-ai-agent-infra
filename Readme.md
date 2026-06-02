# Run this playbook
ANSIBLE_CONFIG=ansible.cfg ansible-playbook wazuh-server-install.yaml -l s-security --ask-vault-pass -i staging.inv

# Set admin user password in wazuh
1. Download tool
curl -so wazuh-passwords-tool.sh https://packages.wazuh.com/4.14/wazuh-passwords-tool.sh
2. generate the password
sudo ./wazuh-passwords-tool.sh -u admin -p 123passord
