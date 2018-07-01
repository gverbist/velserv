# velserv
velserv ip to velbus server.


source can be downloaded at the following link: leachy.homeip.net/velbus/velserv.c
compiles with: gcc -o velserv velserv.c -lpthread

Usage: ./velserv -csfvhV] -d DEVICE] -a ADDRESS] -p PORT]
Tip : try to run as root

-s --server act as server only, gateway will be disabled
when in server mode, the address is always 127.0.0.1
-c --client act as client only, server wil be disabled
-d --device INTERFACE device where the Velbus interface is connected to
default device is: /dev/ttyACM0
-a --address HOST IP address or hostname where to connect to as client
default is 127.0.0.1
-p --port PORT port where to connect
default is 3788
-f --foreground do not run in background
-v --verbose verbose operation, repeat for debugging output
1 general debug, 2-3 com to socket debug, 4-6 server socket debug
-h --help print this help and exit
-V --version print version information and exit
