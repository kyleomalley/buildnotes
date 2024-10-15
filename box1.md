# apt base

apt-get install vim -y

# Certs

sudo apt update
sudo apt install certbot python3-certbot-dns-cloudflare

sudo mkdir /root/.secrets/
sudo nano /root/.secrets/cloudflare.ini

certbot certonly --dns-cloudflare -d box1.ihl.fivetuple.com --dns-cloudflare-credentials /etc/letsencrypt/cloudflare.ini 

certbot certificates

# virsh
```
virsh metadata rocky8-2024-10-13 --config --key tags --uri http://fivetuple.com/tags --edit
virsh metadata rocky8-2024-10-13 --config --key tags --uri http://fivetuple.com/tags
```
# sysprep

sudo virt-sysprep -a rocky8-2024-10-13-clone-3.qcow2   --operations logfiles,ssh-hostkeys,net-hostname,net-hwaddr,tmp-files,user-account
