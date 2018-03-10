En:YaCyOverHTTPS
================

Date: 2013-03-05 19:12:27

new version of stunnel configuration. the old description in the german
version does not work any more because stunnel4 requires key and cert as
separate files

**Neue Seite**

<div>

=Using the YaCy Front-End over HTTPS=\
\
It is possible to put a SSL encoding in front of YaCy to get the YaCy
interface accessible using https. This can easily be done using stunnel
and openssl.\
\
==Installation of openssl and stunnel in debian==\
\
As user root, call:\
apt-get install openssl stunnel\
Then create a ssl certificate:\
cd \~\
openssl req -new -x509 -keyout stunnel-key-pw.pem -out stunnel-cert.pem
-days 3650\
And get rid of the passphrase with\
openssl rsa -in stunnel-key-pw.pem -out stunnel-key.pem\
As user root, copy the key and certificate file to /etc/stunnel/\
mv stunnel-key.pem stunnel-cert.pem /etc/stunnel/\
chmod 600 /etc/stunnel/\*.pem\
To configure stunnel, create the file /etc/stunnel/stunnel.conf with the
following content:\
chroot = /var/lib/stunnel4/\
setuid = stunnel4\
setgid = stunnel4\
pid = /stunnel4.pid\
cert = /etc/stunnel/stunnel-cert.pem\
key = /etc/stunnel/stunnel-key.pem\
output = stunnel.log\
\
\[https\]\
accept = 443\
connect = 8090\
To activate this service, edit the file /etc/default/stunnel4 and change
the value of ENABLED to 1. Finally restart stunnel:\
/etc/init.d/stunnel4 restart\
Now the YaCy search page can be opened at https://localhost

</div>
