# snapd_certbot
Setup SSL using Snapd and Certbot



sudo yum -y install snapd

sudo systemctl enable --now snapd.socket

sudo ln -s /var/lib/snapd/snap /snap

 

sudo dnf remove certbot

sudo snap install --classic certbot

sudo ln -s /snap/bin/certbot /usr/bin/certbot

sudo certbot certonly --apache
