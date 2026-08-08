# git-hub-actions-bastion
What needs to be added manually
```
Go to your repo → Settings → Secrets and variables → Actions → New repository secret, and add:
Secret name	Value	Where it comes from
BASTION_SSH_KEY	Full contents of the bastion's private key .pem file	The key pair you created for the bastion instance
APP_SSH_KEY	Full contents of the app server's private key .pem file	Could be the same key pair as bastion, or a different one
BASTION_IP	Bastion's public IP	tofu output bastion_ip
APP_PRIVATE_IP	App server's private IP	tofu output app_private_ip
```
