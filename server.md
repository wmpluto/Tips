+ apt update
+ apt upgrade
+ wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh
+ addgroup pluto
+ useradd -d /home/pluto -g pluto -s /bin/bash -m pluto
+ passwd pluto
+ vi /etc/sudoers
+ sudo apt install shadowsocks-libev
+ sudo vi /etc/ssh/sshd_config
+ iptables
    + sudo iptables -L -n --line-numbers
    + sudo iptables -D (Number of Line)
    + sudo iptables sudo -A INPUT -p tcp --dport ssh -j ACCEPT
    + sudo iptables sudo -A INPUT -j DROP
    + sudo iptables-save
    + sudo netfilter-persistent save
    + sudo netfilter-persistent reload
+ nvm/node
    + curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.34.0/install.sh | bash
    + nvm install v7.10.0
+ pyenv
    + sudo apt install python3-venv

