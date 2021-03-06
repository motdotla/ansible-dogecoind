# ansible-dogecoind

![](https://raw.github.com/scottmotte/ansible-dogecoind/master/ansible-dogecoind.png)

Run dogecoind on your server of choice to the moon. Designed for Ubuntu 12.04 x64.

([Kibble](https://github.com/scottmotte/kibble) goes well with this repo. So kibble n bits. Maybs.)

If you would like some tip to this shibe: `DJEBk3QoBGbNL7oWzXqvjgW1A9DuFKHs8q`

## Installation

### Digital Ocean

Create a [droplet](https://www.digitalocean.com/?refcode=ebcbc179c33f) on digital ocean and note the IP Address. 

Then on your local machine, run the following.

```
git clone https://github.com/scottmotte/ansible-dogecoind.git
cd ansible-dogecoind
cp dogecoin.conf.example dogecoin.conf 
cp hosts.example hosts
```

Edit the `dogecoin.conf` and `hosts` files.

Deploy using [ansible](http://www.ansibleworks.com). (install instructions for ansible are in [requirements](#requirements) below.

```
ansible-playbook playbook.yml -i hosts
```

That's it. Now dogecoind is running on its own server.

## Requirements

[Ansible](http://www.ansibleworks.com/) is required. 

### Installing Ansible on Mac

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

## History

This project was originally built at [Riverside.io](http://riverside.io)'s [New Years Hackathon 2014](https://www.hackerleague.org/hackathons/riverside-dot-io-new-years-hackathon-2014). If wantz donate Riverside.io: `DRyL99xweAbB1QJggYif6wPTHnn6F35JJK`.

<img src="http://www.rawr.la/images/newyears_poster.jpg" width="500">
