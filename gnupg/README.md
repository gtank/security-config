These files contain references to the pool server's CA cert, which you will
need to configure to point to a copy on your own machine.

# Installation

By default, these files should go in your ~/.gnupg directory.

# Keyserver certificate
The cert is hosted at https://sks-keyservers.net/sks-keyservers.netCA.pem

GnuPG 1.4 and 2.0 users should set the following option in gpg.conf

    keyserver-options ca-cert-file=/path/to/CA/sks-keyservers.netCA.pem

GnuPG 2.1 users should set the following in dirmngr.conf:

    hkp-cacert /path/to/CA/sks-keyservers.netCA.pem

Fingerprints are available at https://sks-keyservers.net/verify_tls.php
