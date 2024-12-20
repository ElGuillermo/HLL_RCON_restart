# HLL_CRCON_restart
Stand alone tool to restart an Hell Let Loose (HLL) CRCON (see : https://github.com/MarechJ/hll_rcon_tool) install.

What it does :  
- `(optional)` rebuild CRCON  
- `(optional)` stop CRCON
- `(optional)` flush Redis cache  
- `(optional)` delete logs  
- restart CRCON  
- `(optional)` delete obsolete Docker containers and images  
- `(optional)` report disk usage of various CRCON components

## Install

> [!NOTE]
> The shell commands given below assume your CRCON is installed in `/root/hll_rcon_tool`.  
> You may have installed your CRCON in a different folder.  
>   
> Some Ubuntu Linux distributions disable the `root` user and `/root` folder by default.  
> In these, your default user is `ubuntu`, using the `/home/ubuntu` folder.  
> You should then find your CRCON in `/home/ubuntu/hll_rcon_tool`.  
>   
> If so, you'll have to adapt the commands below accordingly.

- Log into your CRCON host machine using SSH and enter these commands (one line at a time) :
```shell
cd /root/hll_rcon_tool
wget https://raw.githubusercontent.com/ElGuillermo/HLL_RCON_restart/refs/heads/main/restart.sh
```

## Config
- Edit `/root/hll_rcon_tool/restart.sh` and set parameters to fit your needs.

## Use
- Log into your CRCON host machine using SSH and enter these commands (one line at a time) :
```shell
cd /root/hll_rcon_tool
sudo sh ./restart.sh
```
