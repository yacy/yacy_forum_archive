Dev:EnhancedBase64
==================

Date: 2013-11-22 10:53:41

explanation of YaCy Base 64 for more detailed API description

**Neue Seite**

<div>

There was the necessity to have a base64 encoding of binary objects in
many places in YaCy, but a modified version of the standard
\[http://www.ietf.org/rfc/rfc1521.txt RFC 1521 Base64\] encoding and
decoding has been used.\
\
YaCy uses an \'enhanced base 64 encoding\' which is based on RFC 1521
Base64 with two exceptions:\
\* the characters \'+\' and \'/\' are replaced by \'-\' and \'\_\'
(\'+\' by \'-\' and \'/\' by \'\_\')\
\* the trailing fill-up character \'=\' is omitted\
\
There is a good reason in YaCy to change the RFC 1521 standard:\
\* the base64 encoding result is used as part of file names, and the
characters \'+\' and \'/\' are not accepted as file names in all file
systems\
\* the \'=\' trailing is superfluous and wastes space.\
\
If you want to use the YaCy EnhancedBase64 in other applications or
programming languages then you can convert from EnhancedBase64 to RFC
1521 Base64 with the following steps (enhanced this!):\
String rfc1521 = new String(eb64);\
while (rfc1521.length() % 4 != 0) rfc1521 += \"=\";\
rfc1521 = rfc1521.replace(\'-\', \'+\').replace(\'\_\', \'/\');\
\
If you want to convert from RFC 1521 Base64 to EnhancedBase64, do the
following:\
String eb64 = new String(rfc1521);\
while (eb64.endsWith(\"=\")) eb64 = eb64.substring(0, eb64.length() -
1);\
eb64 = eb64.replace(\'+\', \'-\').replace(\'/\', \'\_\');

</div>
