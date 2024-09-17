# How to install v2raya in centos 7

## We need v2-ray core and v2raya（please switch to root or you add your account in sudoer）

1. add v2ray core 

   Download I uploaded zip format file

   1. put v2ray to  /usr/local/bin/ 

      `mv v2ray /usr/local/bin/  `

      if you don't have this floder

      ``mkdir /usr/local/bin/` 

      make v2ray to executable file  

      `chmod 777 /usr/local/bin/v2ray`

   2. put *.dat to /usr/local/share/v2ray/

      `mv geoip.dat /usr/local/share/v2ray/`  

      `mv geosite.dat /usr/local/share/v2ray/`

3. install v2raya
   `sudo yum install installer_redhat_x64_2.2.4.1.rpm`

4. start v2raya

   `systemctl start v2raya.service`

    Set to start automatically at boot

   `systemctl enable v2raya.service` 

   Restart takes effect

   `systemctl restart v2raya.service`

5. enter web 
   `localhost:2017`

if you forget your password

`v2raya --reset-password` 

