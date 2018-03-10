Dev:SimpleCoding
================

Date: 2013-11-22 11:11:26

explained SimpleEncoding as basis for the explanation of seedlists

**Neue Seite**

<div>

The YaCy API contains some strings which are encoded with a
\'SimpleCoding\' method (from class net.yacy.utils.crypt).\
Strings encoded with the SimpleCoding method have the following form:\
\<encoding-type-char\>\'\|\'\<encoded-ascii\>\
where \<encoding-type-char\> is a single character which selects the
used encoding and \<encoded-ascii\> is the content consisting of ASCII
characters. There is a pipe-symbol (\'\|\') between these two parts. The
pipe symbol can be used as encoding-magic to test if a string is
SimpleEncoded.\
\
The \<encoding-type-char\> can have three different values:\
\'b\' : the \<encoded-ascii\> is an
\[\[Dev:EnhancedBase64\|EnhancedBase64\]\]-encoded String of the
(binary) content\
\'z\' : the \<encoded-ascii\> is an
\[\[Dev:EnhancedBase64\|EnhancedBase64\]\]-encoded String of a
gzip-compressed stream of the (binary) content\
\'p\' : the \<encoded-ascii\> is the (not binary) content (that means
that the encoded content is equal to the \<encoded-ascii\> and not
actually encoded)\
\
Most methods which write SimpleEncoding strings do first an encoding
with and without gzip and compare the size of the output. Sometimes the
gzip-encoded result is larger than the uncompressed result and that is
the basis to choose \'b\' or \'z\'.\
\
Example: a typical SimpleEncoding looks like:\
z\|H4sIAAAAAAAAAD2QT0-DUBDEv0ovetCV7L4\_y2vMXqRWqbUlLXg1JL4oiQXCw5hq\_O7SUj3\_ZmZn5\_vJd6FqaqGILeJUM8MqaT7qXpQjpaYOiravdl4IDSQjMRHCsgz91vtaFJKmQUlIysRQbFvvXwQhFGJZoXUGtqONdAxpJoYjYh1xHDEsTyRWHDuGdDQTxbAZyZCTilVWE8J9Gd5knj27h8VXs6CqhazpenE4Rci87\_J96yX4umo6KPJELpEQYVUO5Wfrx9vV3foKyUD638axYcjL1yAX0KXCbKwxGrpCyBrlDoWyY-i537X9\_ho2p-ciRK0HToOk9p9B4GZW9v5vi-Gucgph\_n7IPptMJj-\_CQ5ytGgBAAA

</div>
