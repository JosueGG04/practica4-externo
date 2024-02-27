# practica4-externo
Repositorio para hacer la practica 4 de programacion web

# Descargar y correr script
wget https://raw.githubusercontent.com/JosueGG04/practica4-externo/main/miScript.sh && chmod +x miScript.sh && bash miScript.sh

# Comandos
## Apache
cd /etc/apache2/sites-available/

sudo a2enmod proxy proxy_html proxy_http

## SSL
sudo a2enmod ssl

sudo service apache2 stop

 
sudo certbot certonly -m jdgg0001@ce.pucmm.edu.do -d app-1.josue04.me

sudo certbot certonly -m jdgg0001@ce.pucmm.edu.do -d app-2.josue04.me

## Iniciar
sudo a2ensite seguro.conf

sudo systemctl restart apache2