# DZ_SYSTEMD


1. задание:

konstantin@konstantin1:/etc/systemd/system$ sudo tail -n 1000 /var/log/syslog  | grep found
Oct  6 03:45:27 konstantin1 root: Mon Oct  6 03:45:27 AM UTC 2025: Word, found!
Oct  6 03:46:27 konstantin1 root: Mon Oct  6 03:46:27 AM UTC 2025: Word, found!
Oct  6 03:47:26 konstantin1 root: Mon Oct  6 03:47:26 AM UTC 2025: Word, found!
Oct  6 03:48:18 konstantin1 root: Mon Oct  6 03:48:18 AM UTC 2025: Word, found!
Oct  6 03:48:48 konstantin1 root: Mon Oct  6 03:48:48 AM UTC 2025: Word, found!
Oct  6 03:49:26 konstantin1 root: Mon Oct  6 03:49:26 AM UTC 2025: Word, found!
Oct  6 03:50:26 konstantin1 root: Mon Oct  6 03:50:26 AM UTC 2025: Word, found!
Oct  6 03:51:25 konstantin1 root: Mon Oct  6 03:51:25 AM UTC 2025: Word, found!




2. задание:

spawn-fcgi.service - Spawn-fcgi startup service by Otus
     Loaded: loaded (/etc/systemd/system/spawn-fcgi.service; disabl>
     Active: active (running) since Sun 2025-10-05 07:13:54 UTC; 2h>
   Main PID: 50403 (php-cgi)
      Tasks: 33 (limit: 2219)
     Memory: 14.2M
        CPU: 25ms
     CGroup: /system.slice/spawn-fcgi.service
             ├─50403 /usr/bin/php-cgi
             ├─50404 /usr/bin/php-cgi
             ├─50405 /usr/bin/php-cgi
             ├─50406 /usr/bin/php-cgi
             ├─50407 /usr/bin/php-cgi
             ├─50408 /usr/bin/php-cgi
             ├─50409 /usr/bin/php-cgi
             ├─50410 /usr/bin/php-cgi
             ├─50411 /usr/bin/php-cgi
             ├─50412 /usr/bin/php-cgi
             ├─50413 /usr/bin/php-cgi
             ├─50414 /usr/bin/php-cgi
             ├─50415 /usr/bin/php-cgi
             ├─50416 /usr/bin/php-cgi
             ├─50417 /usr/bin/php-cgi
             ├─50418 /usr/bin/php-cgi
             ├─50419 /usr/bin/php-cgi
             ├─50420 /usr/bin/php-cgi
             ├─50421 /usr/bin/php-cgi
             ├─50422 /usr/bin/php-cgi
             ├─50423 /usr/bin/php-cgi
             ├─50424 /usr/bin/php-cgi
             ├─50425 /usr/bin/php-cgi
             ├─50426 /usr/bin/php-cgi
             ├─50427 /usr/bin/php-cgi
             ├─50428 /usr/bin/php-cgi
             ├─50429 /usr/bin/php-cgi
             ├─50430 /usr/bin/php-cgi
             ├─50431 /usr/bin/php-cgi
             ├─50432 /usr/bin/php-cgi
             ├─50433 /usr/bin/php-cgi
             ├─50434 /usr/bin/php-cgi
             └─50435 /usr/bin/php-cgi

Oct 05 07:16:19 konstantin1 systemd[1]: /etc/systemd/system/spawn-f>
Oct 05 07:16:20 konstantin1 systemd[1]: /etc/systemd/system/spawn-f>
Oct 05 07:23:02 konstantin1 systemd[1]: /etc/systemd/system/spawn-f>



3. задание:

root@konstantin1:/etc/nginx# ps afx | grep nginx
  52350 pts/1    S+     0:00  |                           \_ grep --color=auto nginx
  52323 ?        Ss     0:00 nginx: master process /usr/sbin/nginx -c /etc/nginx/nginx-second.conf -g daemon on; master_process on;
  52324 ?        S      0:00  \_ nginx: worker process
  52325 ?        S      0:00  \_ nginx: worker process
  52330 ?        Ss     0:00 nginx: master process /usr/sbin/nginx -c /etc/nginx/nginx-first.conf -g daemon on; master_process on;
  52331 ?        S      0:00  \_ nginx: worker process
  52332 ?        S      0:00  \_ nginx: worker process
