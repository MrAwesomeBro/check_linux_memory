# Linux Memory Check for Icinga2

Copy the hosts and template folder to ```/etc/icinga2/conf.d```.

Then Copy the **check_linux_memory** to the nagios-plugins folder:

* Debian/Ubuntu: ```/usr/lib/nagios/plugins```

* RedHat/CentOS: ```/usr/lib64/nagios/plugins```

After that chmod the check file to give it the needed permissions:

* Debian/Ubuntu: ```chmod +x /usr/lib/nagios/plugins/check_linux_memory```

* RedHat/CentOS: ```chmod +x /usr/lib64/nagios/plugins/check_linux_memory```

Now modify the **hosts/yourhost.conf** to your needs and save it.

Finally restart icinga service:

     service icinga2 restart

Or:

    systemctl restart icinga2
