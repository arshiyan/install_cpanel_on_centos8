# install_cpanel_on_centos8
Who to install cpanel WHM on centos
آموزش نصب سی پنل در centos 8


- yum install wget -y
- echo '168.119.126.94 repo.mysql.com yum.mariadb.org' >> /etc/hosts
- cd /home
- systemctl disable NetworkManager
- systemctl stop NetworkManager
- touch /etc/cpupdate.conf
- echo "CPANEL=edge" > /etc/cpupdate.conf
- wget -O latest http://httpupdate.cpanel.net/latest
- chmod +x latest
- sh latest
