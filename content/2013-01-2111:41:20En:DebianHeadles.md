En:DebianHeadless
=================

Date: 2013-01-21 11:41:20

How to shrink Debian if x11 is removed

**Neue Seite**

<div>

==Shrink Debian by removing all graphical features to turn it into a
headless server==\
For YaCy, no online graphical interface is needed. Because YaCy starts
automatically with a headless-option, only a headless java (i.e. package
openjdk-6-jre-headless) is requiret and we can safely remove all grapics
drivers from debian.\
\
===Delete Packages for Graphics===\
As root, simply do\
apt-get remove \--purge libx11-6\
followed by a clean-up\
apt-get autoremove \--purge\
sudo apt-get clean\
This will remove many packages, but to get debian really clean, remove
unused packages as well. This should include all non-headless
applications. Some can be discovered automatically, see next section.\
\
===Remove All Unused Packages===\
Because some unused packages do not necessarily have dependencies to
removed packages, we need a tool to discover such orphaned packages:\
apt-get install deborphan\
deborphan\
deborphan \--guess-all\
\
You can easily remove all packages which deborphan reports with\
apt-get remove \--purge \`deborphan\`\
apt-get remove \--purge \`deborphan \--guess-all\`\
apt-get autoremove \--purge\
Repeat this until no more packages are deleted, then do a\
apt-get clean

</div>
