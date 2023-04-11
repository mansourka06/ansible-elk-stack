# ansible-elk-stack
This repository set up an ELK (Elasticsearch, Logstash, Kibana) Stack installation using Ansible.


## Installing and Configuring the ELK Stack with Ansible
This repository contains an Ansible playbook and associated files for installing and configuring the ELK (Elasticsearch, Logstash, Kibana) stack on a group of Ubuntu servers.

## Prerequisites
- Ansible 2.9 or later installed on the local machine
- Access to a group of Ubuntu servers that you want to install the ELK stack on

## Usage
* 1. Clone this repository to your local machine:
    **git clone https://github.com/mansourka06/ansible-elk-stack.git**

* 2. Update the hosts file in the repository with the IP addresses or hostnames of the servers you want to install the ELK stack in [the inventory file](./hosts.in)

* 3. Update the [vars file](roles/elk-stack/vars/main.yml) with your desired configuration options for the ELK stack.

* 4. Run the Ansible playbook to install and configure the ELK stack on the target servers: 
    **ansible-playbook -i hosts playbook.yml --ask-become-pass**

* 5. After the playbook has completed, you should be able to access the Kibana web interface by navigating to http://<kibana_host>:<kibana_port> in a web browser. The default Kibana URL is http://localhost:5601.


## Author
- ** Mansour KA