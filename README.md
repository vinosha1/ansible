# ansible
Install and Configure Ansible Tower on RHEL/Centos
Ansible exists in two standards:
Ansible Core - Provides Ansible runtime for executing playbooks.
Ansible Tower- Provides managements, visibility, job scheuling, credentials, RBAC, auditing/compliance etc.by installing Ansible Tower, Ansible core will be installed as a deper
installed as a dependency. Below are the steps you'll use to install Ansible Tower on a Centos 7 server.
1.  Update system and add EPEL repostory.
We need the EPEL repository for this installation, update your Centos 7 system and add EPEL repository.
yum -y update
yum -y install epel-release

 install ansible uses Ansible playbook to deploy itself so we also need Ansible installed.
yum -y install ansible vim curl

2.
Download Ansible Tower archive
Download the latest Ansible Tower Release.
mkdir /tmp/tower && cd /tmp/tower
curl -o https://releases.ansible.com/ansible-tower/setup/ansible-tower-setup-latest.tar.gz
Extract download archive.

tar xvf ansible-tower-setup-latest.tar.gz
Step 3: Install Ansible Tower
Navigate to the created dircetory
cd ansible-tower-setup/
$ vim inventory
sudo ./setup. installation of Ansible Tower on Centos 7.
This will invoke Ansible playbook to install Ansible Tower on Cento5 7. If successful, the message like this should show at the end.
