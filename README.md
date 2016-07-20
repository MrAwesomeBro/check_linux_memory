# Linux Memory Check for Icinga2

1. Copy the hosts and template folder to ```/etc/icinga2/conf.d```.

2. Copy the **check_linux_memory** to the nagios-plugins folder:
 * Debian/Ubuntu: ```/usr/lib/nagios/plugins```
 * RedHat/CentOS: ```/usr/lib64/nagios/plugins```

3. Chmod the check file to give it the needed permissions:
 * Debian/Ubuntu: ```chmod +x /usr/lib/nagios/plugins/check_linux_memory```
 * RedHat/CentOS: ```chmod +x /usr/lib64/nagios/plugins/check_linux_memory```

4. Modify the **hosts/yourhost.conf** to your needs and save it.

5. Restart icinga service:

    service icinga2 restart

 Or:

    systemctl restart icinga2
