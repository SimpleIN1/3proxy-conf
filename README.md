# 3proxy

Install 3proxy:
    
    wget https://github.com/z3APA3A/3proxy/releases/download/0.9.3/3proxy-0.9.3.x86_64.deb 
    dpkg -i 3proxy-0.9.3.x86_64.deb

Configure 3proxy settings file.

    vi /etc/3proxy/3proxy.cfg

Add proxy users. Run package mantainer's script to do this:

    /etc/3proxy/conf/add3proxyuser.sh <proxylogin> <proxypassword> <daily_trafic_limit_in_MBs> <network_speed_limit_in_bits_per_second>

Start 3proxy:
    
    systemctl enable 3proxy.service
    systemctl start 3proxy.service
