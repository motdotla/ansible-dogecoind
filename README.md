# ansible-dogecoind

Quickly get dogecoind running on your server using this ansible config.

## Usage

Create a new [droplet](https://www.digitalocean.com/?refcode=ebcbc179c33f) on digital ocean. 

```
cp dogecoin.conf.example dogecoin.conf 
cp hosts.example hosts
```

Edit `dogecoin.conf` and `hosts` with configuration of your choice.

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

Doge Donate: `DJEBk3QoBGbNL7oWzXqvjgW1A9DuFKHs8q`
