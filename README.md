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




now we should run thsi command to make sure our rules are up
```bash
sudo ufw status verbose
```
![Screenshot 2024-04-09 093724](https://github.com/Sabbasnia/acit-2024/assets/148383173/2e5c57dd-dafb-4c5c-84a7-2ae5c0e80d1f)



