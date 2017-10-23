Tree Structure
 |--README
 |--/client
	|--tftp.h
	|--tftp.c
	|--tftpclient.c
 |--/server
	|--tftp.h
	|--tftp.c
	|--tftpserver.c

open two terminals
to compile
1. cd client
2. gcc tftpclient.c -o tftpclient
3. cd server
4. gcc tftpserver.c -o tftpserver


to run the program:
1. for the server side
	cd server
	./tftpserver or ./tftpserver -p portnumber
2. for the client side
	cd client
	./tftpclient -r/-w filename or
           ./tftpclient -r/-w filename -p portnumber


—————————————

I wasn’t able to finish implementing that it would be able to handle the server client folders which were mentioned on piazza to be gradescope compatible. I didn’t want to ruin
my code incase it broke down completely.

I strictly followed the PDF provided to us in class and the test_echo_client.c and server_test.c from a previous year’s website.

I understand why you wanted the ports to be two different values so to check whether when the port numbers were different, nothing was executed and once -p # was specified correctly and the two ports matched the way it should, then there would be a file transfer between the two.
