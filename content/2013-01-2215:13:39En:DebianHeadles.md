En:DebianHeadless
=================

Date: 2013-01-22 15:13:39

[Remove All Unused Packages: ]{.autocomment} more removal tools

← Nächstältere Version

Version vom 22. Januar 2013, 14:13 Uhr

Zeile 10:

Zeile 10:

 

<div>

This will remove many packages, but to get debian really clean, remove
unused packages as well. This should include all non-headless
applications. Some can be discovered automatically, see next section.

</div>

 

<div>

This will remove many packages, but to get debian really clean, remove
unused packages as well. This should include all non-headless
applications. Some can be discovered automatically, see next section.

</div>

 

 

−

<div>

===~~Remove All Unused Packages~~===

</div>

\+

<div>

===[Orphaned Package Removal]{.underline}===

</div>

 

<div>

Because some unused packages do not necessarily have dependencies to
removed packages, we need a tool to discover such orphaned packages:

</div>

 

<div>

Because some unused packages do not necessarily have dependencies to
removed packages, we need a tool to discover such orphaned packages:

</div>

 

<div>

  apt-get install deborphan

</div>

 

<div>

  apt-get install deborphan

</div>

Zeile 22:

Zeile 22:

 

<div>

Repeat this until no more packages are deleted, then do a

</div>

 

<div>

Repeat this until no more packages are deleted, then do a

</div>

 

<div>

  apt-get clean

</div>

 

<div>

  apt-get clean

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[===Remove Large Packages===]{.underline}

</div>

 

\+

<div>

[This goes beyond removal of non-headless software but might be useful
to further shrink debian to get away large and unused software. You can
easily discover large packages with]{.underline}

</div>

 

\+

<div>

[dpkg-query -W \--showformat=\'\${Installed-Size} \${Package} \[depends:
\${Depends}\]\\n\' \| sort -n]{.underline}

</div>

 

\+

<div>

[which lists each package with occupied kilobytes, the package name and
the dependencies for that package. A good starting point is the removal
of large packages with many dependencies because chances are high that
then again orphaned packages appear which can be removed with the
\'Orphaned Package Removal\' from last section.]{.underline}

</div>

 

\+

<div>

[]{.underline}

</div>

 

\+

<div>

[===Remove Software with Large Runtime===]{.underline}

</div>

 

\+

<div>

[Some software on your server may consume a lot of CPU time. If some of
these processes are of no use for you, you can delete them. To discover
such processes, run]{.underline}

</div>

 

\+

<div>

[top -bn1 \| grep root \| sort -k11]{.underline}

</div>

 

\+

<div>

[Whenever you removed more packages, run the \'Orphaned Package
Removal\' process again.]{.underline}

</div>
