Tempest sidechannel attacks now cheaper
=======================================

Date: 2015-06-25 02:33:17

[![](http://www.jwz.org/images/em-rattlew-n200-w800.png)![](http://www.jwz.org/images/n200-manykeys-em-h500.png)Stealing
Keys from PCs using a Radio: Cheap Electromagnetic Attacks on Windowed
Exponentiation](https://www.tau.ac.il/~tromer/radioexp/)

> We demonstrate the extraction of secret decryption keys from laptop
> computers, by nonintrusively measuring electromagnetic emanations for
> a few seconds from a distance of 50 cm. The attack can be executed
> using cheap and readily-available equipment: a consumer-grade radio
> receiver or a Software Defined Radio USB dongle. \[\...\]
>
> We successfully extracted keys from laptops of various models running
> GnuPG (popular open source encryption software, implementing the
> OpenPGP standard), within a few seconds. The attack sends a few
> carefully-crafted ciphertexts, and when these are decrypted by the
> target computer, they trigger the occurrence of specially-structured
> values inside the decryption software. These special values cause
> observable fluctuations in the electromagnetic field surrounding the
> laptop, in a way that depends on the pattern of key bits
> (specifically, the key-bits window in the exponentiation routine). The
> secret key can be deduced from these fluctuations, through signal
> processing and cryptanalysis.

[Previously](http://www.jwz.org/blog/2014/01/quietnet/),
[previously](http://www.jwz.org/blog/2004/12/optical-tempest/).
