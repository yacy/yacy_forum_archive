En:FreeBSDInstall
=================

Date: 2014-12-14 15:31:40

add initial version

**Neue Seite**

<div>

== FreeBSD Install Guide ==\
\
=== Requirements ===\
\
Next to Java YaCy requires bash and either wget or curl to work. These
are used for the scripts you find in ./bin. So we install those via pkg
or ports\
\
\<pre\>\
\# Using pkg:\
pkg install openjdk curl bash\
\</pre\>\
\
==== Java Setup ====\
\
Java requires proc and fd to be mounted. Make sure to append these lines
to /etc/fstab\
\
\<pre\>\
fdesc /dev/fd fdescfs rw 0 0\
proc /proc procfs rw 0 0\
\</pre\>\
\
Then reboot or mount them manually for the changes to take effect.\
\
=== Install YaCy ===\
\
For security reasons you should run YaCy as its own user. So you might
want to add a user called YaCy and switch to it.\
\
\<pre\>\
\# As root:\
adduser\
Username: yacy\
\...\
\# Switch to user yacy\
su - yacy\
\</pre\>\
\
You need to download and extract the Linux version of YaCy. Luckily it
does not seem to be Linux specific at all.\
\<pre\>\
curl -o yacy.tar.gz
http://www.yacy.net/release/yacy\_\<CURRENT\_RELEASE\>.tar.gz \# Replace
CURRENT\_RELEASE with whatever the current version is\
tar xzvf yacy.tar.gz\
\</pre\>\
\
That\'s it! You can now cd into directory and start YaCy.\
\<pre\>\
cd yacy\
./startYACY.sh\
\</pre\>\
\
=== Side notes for YaCy developers and advanced users ===\
\
To make the installation easier \"/usr/bin/env bash\" in various scripts
should be replaced with \"/usr/bin/env sh\". Bash doesn\'t seem to be
required for scripts to work,\
so this would remove an explicit dependency. FreeBSD comes with ftp
(which also supports http) and fetch, which could theoretically be used
in bin/apicall.sh. However\
the way the password is sent (using MD5:\...) appears to be causing
problems. I was not yet able to work around this. If this could be fixed
curl/wget would not be required.

</div>
