En:DebianHeadless
=================

Date: 2013-04-18 10:46:00

[Remove Software with Large Runtime: ]{.autocomment} Remove Old Kernel
Modules

← Nächstältere Version

Version vom 18. April 2013, 08:46 Uhr

(2 dazwischenliegende Versionen von einem Benutzer werden nicht
angezeigt)

Zeile 32:

Zeile 32:

 

<div>

  top -bn1 \| grep root \| sort -k11

</div>

 

<div>

  top -bn1 \| grep root \| sort -k11

</div>

 

<div>

Whenever you removed more packages, run the \'Orphaned Package Removal\'
process again.

</div>

 

<div>

Whenever you removed more packages, run the \'Orphaned Package Removal\'
process again.

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[===Remove Old Kernel Modules===]{.underline}

</div>

 

\+

<div>

[Kernel modules take up a large disk space and can easily be removed. To
ensure that you are doing the right thing, first check which kernel you
are running with]{.underline}

</div>

 

\+

<div>

[uname -r]{.underline}

</div>

 

\+

<div>

[Then you can look for the modules which are stored with]{.underline}

</div>

 

\+

<div>

[ls /lib/modules]{.underline}

</div>

 

\+

<div>

[Finally remove the modules, which are not identical to the one as
discovered with uname -r using i.e.]{.underline}

</div>

 

\+

<div>

[apt-get remove \--purge 3.5.0-17-generic]{.underline}

</div>

 

\+

<div>

[and so on for all old kernel. This will free about 100MB of disk space
for each kernel.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[===Search for installed packages===]{.underline}

</div>

 

\+

<div>

[Whenever you want to remove a package, you must know the name of that
package. The package names of all installed packages can be listed
with]{.underline}

</div>

 

\+

<div>

[dpkg \--get-selections]{.underline}

</div>

 

\+

<div>

[This can be useful i.e. if you want to see if you have two versions of
the same tool, i.e.]{.underline}

</div>

 

\+

<div>

[dpkg \--get-selections \*jre\*]{.underline}

</div>

 

\+

<div>

[may show you that you have installed jre-6 and jre-7, so you can remove
one of them.]{.underline}

</div>

 

 

 

<div>

===Prepare for tiny VirtualBox ova Appliance Dumps===

</div>

 

<div>

===Prepare for tiny VirtualBox ova Appliance Dumps===

</div>

Zeile 41:

Zeile 57:

 

<div>

  rm -Rf /usr/share/doc

</div>

 

<div>

  rm -Rf /usr/share/doc

</div>

 

<div>

  rm -Rf /usr/share/man

</div>

 

<div>

  rm -Rf /usr/share/man

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[As a very last step you can also delete the package lists]{.underline}

</div>

 

\+

<div>

[rm -r /var/lib/apt/lists]{.underline}

</div>

 

\+

<div>

[.. which will free about 100MB of disk space. The lists directory is
recreated the next time you run apt-get update.]{.underline}

</div>

 

 

 

<div>

====Wipe Out Empty Space====

</div>

 

<div>

====Wipe Out Empty Space====

</div>
