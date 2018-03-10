Quellcodekommentar der Woche, aus dem OpenBSD-Cleanup \...
==========================================================

Date: 2014-04-16 16:41:43

Quellcodekommentar der Woche, [aus dem OpenBSD-Cleanup von
OpenSSL](http://www.openbsd.org/cgi-bin/cvsweb/src/lib/libssl/src/apps/asn1pars.c?rev=1.15):

    spray the apps directory with anti-VMS napalm.
    so that its lovecraftian horror is not forever lost, i reproduce below
    a comment from the deleted code.

            /* 2011-03-22 SMS.
             * If we have 32-bit pointers everywhere, then we're safe, and
             * we bypass this mess, as on non-VMS systems.  (See ARGV,
             * above.)
             * Problem 1: Compaq/HP C before V7.3 always used 32-bit
             * pointers for argv[].
             * Fix 1: For a 32-bit argv[], when we're using 64-bit pointers
             * everywhere else, we always allocate and use a 64-bit
             * duplicate of argv[].
             * Problem 2: Compaq/HP C V7.3 (Alpha, IA64) before ECO1 failed
             * to NULL-terminate a 64-bit argv[].  (As this was written, the
             * compiler ECO was available only on IA64.)
             * Fix 2: Unless advised not to (VMS_TRUST_ARGV), we test a
             * 64-bit argv[argc] for NULL, and, if necessary, use a
             * (properly) NULL-terminated (64-bit) duplicate of argv[].
             * The same code is used in either case to duplicate argv[].
             * Some of these decisions could be handled in preprocessing,
             * but the code tends to get even uglier, and the penalty for
             * deciding at compile- or run-time is tiny.
             */

Da ist man auch als Atheist versucht, nach dem Weihwasser zu greifen.
