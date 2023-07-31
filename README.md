## Automated Nexus Deployment using Ansible



**To deploy Nexus using Ansible, follow these steps:**

1. Make sure you have Ansible installed on your system. 

2. Update the `inventory` file with the target hosts where Nexus will be deployed. The file should contain the IP addresses or hostnames of the target servers.

3. Replace `/path/to/your/private-key` in the command below with the actual path to your SSH private key, which will be used to access the target hosts.

4. Run the following command to start the playbook:

```bash
ansible-playbook -i inventory --private-key /path/to/your/private-key deploy-nexus.yaml
```