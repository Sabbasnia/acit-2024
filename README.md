# acit-2024
assignment3par2

first install package

``` bash 
sudo pacman -s ufw
```

after installing ufw you need to allow ssh and http befor enableing the service.


```bash
sudo ufw allow SSH
sudo ufw allow http
```
then we should enable our firewall. this will create a firewall

after adding the rules you must reboot your systemc with the following command. 

```bash
sudo reboot
```

once the system started it then you can activate the ufw firewall here


```bash
sudo ufw enable
```






