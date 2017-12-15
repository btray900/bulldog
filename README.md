# bulldog

## Obtain IP from the console 

I could not get an IP on VMware Workstation so this is done on VirtualBox

![Alt text](./bulldog1.png?raw=true)


## nmap

Scan with nmap. Port 23 is actually SSH. Port 80/8080 is vulnerable.

![Alt text](./bulldog-nmap.png?raw=true)

SSH banner

![Alt text](./bulldog2.png?raw=true)


## dirb

Admin and dev directories found with dirb common wordlist.

![Alt text](./bulldog3.png?raw=true)

![Alt text](./bulldog4.png?raw=true)

The dev page has hashes in the source.

![Alt text](./bulldog5.png?raw=true)


## JtR

The hashes are raw-sha1, and crackable with rockyou.

Compromised credentials: nick:bulldog

![Alt text](./bulldog6.png?raw=true)

![Alt text](./bulldog7.png?raw=true)


## Borwse to admin dir

![Alt text](./bulldog8.png?raw=true)




