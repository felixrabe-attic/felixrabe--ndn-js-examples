# NDN.js examples

For more information on NDN in general, see http://named-data.net/.


## Install and run NFD

Install NFD, then run `nfd-start`.


## Run the examples

    npm install
    node fetch.js

The output should look like:

    Express name /
    1411992371.546245 INFO: [FaceTable] Added face id=257 remote=tcp4://127.0.0.1:53974 local=tcp4://127.0.0.1:6363
    Data received in callback.
    Name: /localhost/nfd/faces/events/%FE%04
    Content: �9�irtcp4://127.0.0.1:53974�tcp4://127.0.0.1:6363�
    NAME: /localhost/nfd/faces/events/%FE%04

    CONTENT(ASCII): À9Áirtcp4://127.0.0.1:53974tcp4://127.0.0.1:6363Â

    CONTENT(hex): c039c10101690201017216746370343a2f2f3132372e302e302e313a35333937348115746370343a2f2f3132372e302e302e313a36333633c20103

    Signature(hex): 08dc85eecef229adc7820c7ad5fd810caadd87c4668f532e80b3b4a0994ed8ad42109f0faa96be1e187867696f4a64f3fdd003fa26e110aa701e0793c52bc9e01798ee7f0b2fd7088ff37dcee8f07af729111ff092684b2eb04604019343e4cdf28ea5d4de2a5dd2dbd16ce9c3beb777039bb32d21e83bfc68d755cee8f3bd0d2bad4eebad4d48de57b575b1ff39150a9592c4b8226501225c6d9367b0ea8c765fe65398a35e3ba702f6e9a807bae9f1b9da7ea156fefdf67e2402d44b0307f017ef12a447179e5c65411b7e7e263837a0fbd15b1375813275dcee3422c5a23cc0bf2b88cce4b0d5fb0ba1bdcb636e8c141b4c9981f5154148f19bb2fa9a1cda

    Publisher Public Key Digest(hex): aa1c3cada4a6f6b173ff68fc85a8c0724bff8b543ee5b81a0e823125804276f6

    TimeStamp: Mon Sep 29 2014 12:06:11 GMT+0000 (UTC)
    TimeStamp(number): 1411992371559
    keyLocator: KeyName: /tmp-identity/%9DA%5E%F0/KEY/ksk-1411992031374/ID-CERT

    Quit script now.
    1411992371.573198 INFO: [TcpLocalFace] [id:257,uri:tcp4://127.0.0.1:53974] Connection closed
    1411992371.578310 INFO: [FaceTable] Removed face id=257 remote=tcp4://127.0.0.1:53974 local=tcp4://127.0.0.1:6363

If you only see

    Express name /

then NFD is not running.
