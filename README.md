**Update and install prerequisites:**
apt update && apt install git nginx -y

**Clone your Git repository:**
git clone https://github.com/shubham-ajbale/Book-Site-The-Hug.git

**Copy your site to Nginx’s web directory:**
rm -rf /var/www/html/*
cd /Book-Site-The-Hug/mybooksite/
cp * /var/www/html/

**Restart Nginx:**
sudo systemctl restart nginx
sudo systemctl status nginx

**Open the site in your browser:**
http://<Public-IP>
