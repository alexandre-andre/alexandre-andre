sudo systemctl stop mariadb
sudo systemctl disable mariadb
yay -Rns mariadb
sudo rm -rf /var/lib/mysql
yay -S mariadb
sudo mariadb-install-db --user=mysql --basedir=/usr --datadir=/var/lib/mysql
sudo systemctl enable mariadb
sudo systemctl start mariadb
sudo mariadb -u root
