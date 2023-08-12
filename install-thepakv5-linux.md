# INSTALLING THEPAKV5 IN LINUX <br><hr>
## UBUNTU section <hr>
first before you install thepakv5 make sure you install wget,git,curl.<br>
```
sudo apt update && sudo apt upgrade -y &&\
sudo apt install wget curl git -y
```
> well if you in ubuntu add mysql-client for fix sql issue

if done try download follow belo
1. clone this repo <br> `git clone --depth 1 https://github.com/TheUnknownName/thepakv5 $HOME/thepakv5`
2. after done,goto to thepakv5 folder.<br> `cd $HOME/thepakv5`
3. after that download this file and make sure this `setupv5.sh` was inside thepakv5 folder<br> ```wget http://mytool.tun06.tech/setupv5.sh-x86_64 -O $HOME/thepakv5/setupv5.sh```
4. after that give permission to be can execute by <br> ```chmod +x $HOME/thepakv5/setupv5.sh```
5. now make bin file thepak `/usr/bin` to execute thepakv5 throught command.just paste it and execute it<br> 
```
sudo cat > $PREFIX/bin/thepak <<- help
#!/bin/bash
if [ -f $rumah/setupv5.sh ];then
    $rumah/setupv5.sh
else
    echo "try reinstalling the thepakv5"
    exit 1
fi
if [ -f $rumah/thepakv5.sh ];then
    $rumah/thepakv5.sh
else
    echo "try reinstalling the thepakv5"
    exit 1
fi
help
sudo chmod +x $PREFIX/bin/thepak
```
6. All done,now execute throught `thepak` command