# Guide of Installation & Configuration

First we have all the information about the project.

```
Gateway: 172.16.0.1/16

Computers must be in range 172.16.1.x/16

And devices must be in 172.16.2.x/16

DHCP has to be disabled
```

> [Change IP in computer](#change-the-ip-in-the-computer)

> [Change IP in printers](#change-the-ip-in-printers)

## Change the IP in the computer

Now we have to change the IPv4 of our PC to a static one.
You can go to settings then press Network & Internet,
when you here. You have to press Ethernet and in IP
assignment, you must provide some stuff.

First we are going to type the DNS server;
In this example I'm going to use the Google DNS server

```
Preferred: 8.8.8.8
Alternative: 8.8.4.4
```

Then type the IP address we want to use as static, but make sure other device doesn't have the same IP address

The IP must be like this `172.16.1.x`

In the subnet mask is going to be `255.255.0.0`
The subnet mask is a series of bits used to separate the network portion from the host portion in an IP address.
In this case the /16 indicates the 16 first bits in the address.

And last we have to put the Gateway that is `172.16.0.1`

With this all config you press save, and you will have a static IP
with DNS server of Google.

This is so helpful to printers and other devices that you want
to use very frequency

## Change the IP in printers
