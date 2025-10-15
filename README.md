apt update && apt install git nginx -y 

git clone https://github.com/shubham-ajbale/Book-Site-The-Hug.git

rm -rf /var/www/html/*

cd /Book-Site-The-Hug/mybooksite/
 
cp * /var/www/html/

systemctl restart nginx
 
systemctl status nginx

http://<Public-IP>
