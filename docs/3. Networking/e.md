# Lan Segments
There is a final network option called a LAN segment. This is an Ethernet segment which has no other functionality and no connection to the host or to the external network. You can join VMs to it and it is the same as connecting them to an unmanaged switch. Any VM on a LAN segment will need a static IP address; alternatively, one of your VMs should be a DHCP server. 

## Exercise
Create a LAN segment and move two VMs to it. Ensure they have static IP information and test that they can ping each other.