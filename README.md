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

then we are recieving the server file from the attachments and bringing to the server



```bash 
 put C:\Users\abbas\Downloads\hello-server
```

after the file of the hello-server passed from ![Screenshot 2024-04-09 100028](https://github.com/Sabbasnia/acit-2024/assets/148383173/899899cb-0ed8-4e22-8e37-a7f8a6cc35a0)
our server to the server we can change the permission for that file 

