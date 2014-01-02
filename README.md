# ansible-dogecoind

Quickly get dogecoind running on your server using this ansible config.

## Usage

```
cp dogecoin.conf.example dogecoin.conf 
cp hosts.example hosts
```

Edit the settings in `dogecoin.conf` and add the server addresses you are deploying to in `hosts`.

Deploy.

```
ansible-playbook playbook.yml -i hosts
```

## Requirements

[Ansible](http://www.ansibleworks.com/) is required.

Install:

```
cd /tmp
git clone git://github.com/ansible/ansible.git
cd ./ansible
git checkout v1.4.3
sudo make install
sudo easy_install jinja2 
sudo easy_install pyyaml
sudo easy_install paramiko
```
