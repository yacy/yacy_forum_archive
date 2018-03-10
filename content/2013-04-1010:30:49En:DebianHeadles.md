En:DebianHeadless
=================

Date: 2013-04-10 10:30:49

[Remove Software with Large Runtime: ]{.autocomment} added more reduce
data and virtual box hints

← Nächstältere Version

Version vom 10. April 2013, 08:30 Uhr

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

[===Prepare for tiny VirtualBox ova Appliance Dumps===]{.underline}

</div>

 

\+

<div>

[To further shrink the debian installation (i.e. to prepare an appliance
dump in VirtualBox), it makes sense to remove more never-used
applications and data.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[====Reduce Data====]{.underline}

</div>

 

\+

<div>

[http://wiki.debian.org/ReduceDebian has some hints to reduce debian,
this is what removes most of the remaining data:]{.underline}

</div>

 

\+

<div>

[rm -Rf /usr/share/locale]{.underline}

</div>

 

\+

<div>

[rm -Rf /usr/share/doc]{.underline}

</div>

 

\+

<div>

[rm -Rf /usr/share/man]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[====Wipe Out Empty Space====]{.underline}

</div>

 

\+

<div>

[When you export a virtual machine to a ova Appliance dump, the virtual
disk is compressed. To enhance this process, it is necessary to zero all
empty disk space. The easiest way to do this is:]{.underline}

</div>

 

\+

<div>

[dd if=/dev/zero of=/emptyspace]{.underline}

</div>

 

\+

<div>

[rm -rf /emptyspace]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[====Shrink Virtual Disk Image====]{.underline}

</div>

 

\+

<div>

[VirtualBox has some command-line tools, this is what you would like to
do to reduce the disk size after you wiped out the empty
space:]{.underline}

</div>

 

\+

<div>

[VBoxManage modifyhd \--compact my\_disk\_image.vdi]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[In case that you created the virtual machine from a ova dump, you
probably don\'t have a vdi file but a vmdk file. This cannot be shrinked
with VBoxManage, but you can create a vdi file out from the vmdk which
can be shrinked then:]{.underline}

</div>

 

\+

<div>

[VBoxManage clonehd \--format vdi my\_disk\_image.vmdk
my\_disk\_image.vdi]{.underline}

</div>

 

\+

<div>

[When doing this, you must assign the new disk to the virtual machine in
the VirtualBox GUI. However, a shrinked vmdk file is mostly smaller than
a shrinked vdi file, therefore it does not make sense to apply this on
an already shrinked appliance.]{.underline}

</div>
