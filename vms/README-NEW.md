```bash
packer build ubuntu1604-ansible.json
vagrant box remove file://../../builds/ubuntu1604-ogs.box # otherwise not reloaded!!
vagrant up

vagrant ssh

cd /vagrant/ansible
ansible-playbook -i "localhost," -c local ogs.yml
```
