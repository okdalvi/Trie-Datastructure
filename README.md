Trie-Datastructure
==================

A trie datastructure for mapping addresses (DNS to IP to MAC)

 Program supports the following commands.
ARPinput <filename> - Loads the input file <filename> which is in the format as explained
above
GetIPAddress <symbolicname> - Returns the IP address(es) that correspond to the
symbolic name <symbolicname>
GetARPAddress <IPaddress> - Returns the MAC address that corresponds to the
IPaddress <IPaddress>
For example, if the input file is named arplookup.txt, then the command
ARPInput arplookup.txt - Loads the input file arplookup.txt which is in the format as
explained above
Consider one of the entries to be www.ecc.ncsu.edu;152.1.1.10;01:02:03:04:05:00
GetIPAddress www.ecc.ncsu.edu - Returns 152.1.1.10
GetARPAddress 152.1.1.10 – Returns 01:02:03:04:05:00
Please note that the input file against which your program is tested can contain a maximum of
1,000,000,000 entries.


Instructions(compile and run):

There are two jar files
1. dnslookup.jar
2. iparp.jar

1. This is the first deliverable. On the command line execute 
	java -jar dnslookup.jar
   To load the input file, type the command, 
	dnsinput <inputfilename>
   Next, to search for the ip address, type
	getipaddress <domain-name> 

2. This is the second deliverable. On the command line execute
	java -jar iparp.jar
   To load the input file, type the command,
	arpinput <inputfilename>
   Next, to search for the ip address, type
	getipaddress <domain-name>
   Next, to search for the arp address from ip address, type
	getarpaddress <ip-address>

Programming Language:
	Java (version 1.7.0_40)
	64 bit Server VM
	
	Note: This code requires a lot of Virtual/Main memory to be present on the machine.Make sure that the machine 
	has more than 4GB of Main as well as Virtual memory available	and it is made available to the program using the 
	command line argument -Xmx4096m if the code goes out of memory.
	
