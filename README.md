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
 ### Starting the firewall and allowing the port 11211 to access memcache (Optional)
~~~
systemctl enable firewalld
~~~
~~~
systemctl start firewalld
~~~
~~~
systemctl status firewalld
~~~
~~~
firewall-cmd --add-port=11211/tcp --permanent
~~~
~~~
firewall-cmd --reload
~~~
~~~
memcached -p 11211 -U 11111 -u memcache -d
~~~
