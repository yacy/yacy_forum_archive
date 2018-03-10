Dev:EnhancedBase64
==================

Date: 2013-11-22 10:55:34

← Nächstältere Version

Version vom 22. November 2013, 09:55 Uhr

Zeile 9:

Zeile 9:

 

<div>

\* the \'=\' trailing is superfluous and wastes space.

</div>

 

<div>

\* the \'=\' trailing is superfluous and wastes space.

</div>

 

 

−

<div>

If you want to use the YaCy EnhancedBase64 in other applications or
programming languages then you can convert from EnhancedBase64 to RFC
1521 Base64 with the following steps (~~enhanced~~ this!):

</div>

\+

<div>

If you want to use the YaCy EnhancedBase64 in other applications or
programming languages then you can convert from EnhancedBase64 to RFC
1521 Base64 with the following steps ([enhance]{.underline} this!):

</div>

 

<div>

  String rfc1521 = new String(eb64);

</div>

 

<div>

  String rfc1521 = new String(eb64);

</div>

 

<div>

  while (rfc1521.length() % 4 != 0) rfc1521 += \"=\";

</div>

 

<div>

  while (rfc1521.length() % 4 != 0) rfc1521 += \"=\";

</div>
