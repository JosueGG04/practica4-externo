# practica4-externo
Repositorio para hacer la practica 4 de programacion web


# Comandos
cd /etc/apache2/sites-available/

sudo a2enmod proxy proxy_html proxy_http

 
sudo a2enmod ssl

sudo service apache2 stop

 
sudo certbot certonly -m jdgg0001@ce.pucmm.edu.do -d app1.josue04.me

sudo certbot certonly -m jdgg0001@ce.pucmm.edu.do -d app2.josue04.me
 

sudo a2ensite seguro.conf

sudo systemctl restart apache2