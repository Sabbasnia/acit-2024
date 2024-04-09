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


```bash
sudo chmod +x hello-server
```
first we need to ```cd /etc/systemd/system```
then we should create a new file for our service for example hello_server.service.
then we have the following 
ExecStart should be path of the hello_server that we will run from the /local/usr/bin
```
[Unit]
Description=Hello Server Service
After=network.target

[Service]
ExecStart=/usr/local/bin/hello-server
Restart=always

[Install]
WantedBy=multi-user.target


```
then we should start our created service  with 
``` bash
sudo systemctl start hello_server.service
```

then you should change your nginx config



![Screenshot 2024-04-09 101435](https://github.com/Sabbasnia/acit-2024/assets/148383173/fa31bb51-e412-48a1-9474-a1f36db19d4c)


in the nginx-2024, we should change the nginx config.

cd to /etc/nignx/sites-availble and change your config file accordingly
![firstone](https://github.com/Sabbasnia/acit-2024/assets/148383173/c7e572ac-250b-4782-81de-02b1df50fbb3)


please restart or reload your nginx
```bash
sudo systemctl restart nginx
```

![Screenshot 2024-04-09 102513](https://github.com/Sabbasnia/acit-2024/assets/148383173/d420193d-d27f-47a5-b098-1382dafa8358)



![thrid](https://github.com/Sabbasnia/acit-2024/assets/148383173/3f48876e-e64f-4fec-a8a9-414cbc5bd11e)





