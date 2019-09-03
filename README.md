# Host Check (ping)

This function is useful for checking whether or not a host is available on the network. This is not necessarily the same device with which your application eventually tries to communicate; for example, perhaps you just want to verify that a certain router along the way is alive. Or perhaps you want your application to scan several IP addresses and issue an alert if any of them drops off the network.

For those kind of situations, we have created the "ping" function. We called it "ping" for conveniece, not because it's actually ICMP-compliant PING (it's not).

With this function, you are able to write something like **HostExist = ping("192.168.0.5",80)** and HostExist would be set "yes" if there's a host on the other end and its port 80 is responding to connection requests (and "no" otherwise). Simple!

