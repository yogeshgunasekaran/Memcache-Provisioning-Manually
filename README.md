# Memcache-Provisioning-Manually
Installation of Memcached in CentOS7
### Install, start & enable memcache on port 11211
 ```sh
  sudo su -
 ```
 ```sh
  yum install epel-release -y
   ```
 ```sh
  yum install memcached -y
   ```
 ```sh
  systemctl start memcached
   ```
 ```sh
  systemctl enable memcached
 ```
 ```sh
  systemctl status memcached
 ```
 ```sh
  memcached -p 11211 -U 11111 -u memcached -d
 ```
