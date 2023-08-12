# FIXING APACHE2 NOT WORKING <HR>
## UBUNTU ENV / LINUX ENV <hr>
if your apache from xampp wasnt working try stop apache2 
1. akses root mode by `sudo su `
2. goto `/etc/init.d` by `cd /etc/init.d/`
   > if you try to ls there will be found apache2
   > <br>thats mean you not install apache2
   > <br>fix by `sudo apt install apache2`
3. then type `./apache2 stop` then automaticly stop the apache2
4. after that you can start xampp normally <br>
**[THANKS TO SAMMY FROM UBUNTU FORUM](https://askubuntu.com/a/463693)**

## WINDOWS (WIP)