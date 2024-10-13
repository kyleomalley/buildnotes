# Certs

sudo apt update
sudo apt install certbot python3-certbot-dns-cloudflare

sudo mkdir /root/.secrets/
sudo nano /root/.secrets/cloudflare.ini

certbot certonly --dns-cloudflare -d box1.ihl.fivetuple.com --dns-cloudflare-credentials /etc/letsencrypt/cloudflare.ini 

certbot certificates
