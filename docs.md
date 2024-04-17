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

> [Open a port in router](#open-the-ports-in-the-router)

> [Open a port](#Open-the-ports-to-remote-access)

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


## Open the ports to remote access
In this example we are going to open the port `22080` to allow external
conexions and remote access.

First we need to go to fire wall and then you navigate to advanced settings

here are some rules, you have to select join rules and press new rule.


Now we select the type, in this case we are going to choose port.
Select TCP for this conection and the port to open is `22080`.

Select allow conection if its save and press next.

we are going to skip this step, but if you want to choose the users can use
this you can and same with the next step.

In this step select all check box.

In the name you can choose whereever you want and same for the description.

Now you can use the port to send conection.


## Open the ports in the router