# bulldog

## obtain IP from the console 

I could not get an IP on VMware Workstation so this is done on VirtualBox.

![Alt text](./bulldog1.png?raw=true)


## nmap

Scan with nmap. Port 23 is actually SSH. Port 80/8080 is vulnerable.

![Alt text](./bdog-nmap.png?raw=true)

SSH banner

![Alt text](./bulldog2.png?raw=true)


## dirb

Admin and dev directories found with dirb common wordlist.

![Alt text](./bulldog3.png?raw=true)

![Alt text](./bulldog4.png?raw=true)

The dev page has hashes in the source.

![Alt text](./bulldog5.png?raw=true)


## john

The hashes are raw-sha1, and crackable with rockyou.

Compromised credentials: nick:bulldog

![Alt text](./bulldog6.png?raw=true)

![Alt text](./bulldog7.png?raw=true)


## browse to admin dir

Login with nick:bulldog.

![Alt text](./bulldog8.png?raw=true)


## browse to webshell

Web shell allowed commands are vulnerable.

![Alt text](./bulldog-webshell.png?raw=true)


## msfvenom

Create a payload for download.

![Alt text](./bulldog9.png?raw=true)


## webshell

Put the file on the target, and execute.

![Alt text](./bulldog10.png?raw=true)

![Alt text](./bulldog11.png?raw=true)

![Alt text](./bulldog12.png?raw=true)

![Alt text](./bulldog13.png?raw=true)

![Alt text](./bulldog14.png?raw=true)


## netcat

Get low priv shell from the target.

![Alt text](./bulldog15.png?raw=true)


## enumerate

Do all the enumeration until you find the hidden directory. Locate the note and the binary. Use 'strings' to discover the potential password. Copy, chmod and execute.

![Alt text](./bulldog16.png?raw=true)

![Alt text](./bulldog17.png?raw=true)

![Alt text](./bulldog18.png?raw=true)

![Alt text](./bulldog19.png?raw=true)


## root

<html><pre>
\(*_*)
  ( (>
  /  \
  </pre></html>


![Alt text](./bulldog20.png?raw=true)


## capture the flag

Done and done...

![Alt text](./bulldog21.png?raw=true)


##  thanks!

Thanks out to Nick F. for the VM.
