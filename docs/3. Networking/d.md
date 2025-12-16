# Bridged Network
This exercise requires administrator privildge, you cannot carry it out on University laboratory computers.

1. In VMWare Workstation, set your Client VM to connect to the bridged LAN, this is normally VMNet0.
2. Start the Client VM and let it boot.
3. Use __ip a__ to identify your IP address.

Draw the network from the perspective of the GUI VM; What can you connect to?

Note that the bridged only network can cause disruption on the host’s LAN and you should not use it without first discussing with your lecturer. If you have more than one network card, you can have more than one bridged network.

<figure>
<img src = "https://jor-donegal.github.io/VMWareWorkstation26/images/fig4.png">
<figcaption>Fig 4. Bridged Network</figcaption>
</figure>

In Fig 4, I manually set vmnet0 to a built-in network card. I then created a new vmnet2 and manually bridged it to a separate network card. I can select either vmnet in each of my VMs, or I can add a virtual network adapter and use both.