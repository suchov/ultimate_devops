# Readme to a course on Udemy

https://www.udemy.com/course/the-complete-devops-bootcamp





# Thoughts

## Routing

I'm on a switching part.
Switch creates a network containing 2 systems.

Router to connect between tho networks.
And a switch to connect within a network - between two systems.

```ip link``` command to connect
```ip addr add 192.168.1.10/24 dev eth0``` - assigne the system with the addresses on the
same network

Router get assigned 2 ip addresses - 1 in each network.
Router is just another device, so we configure the "gateway" or "route"

```route``` command displays the current routing table

```ip route show``` as on iOS ```route -n``` does not work

```ip route add 192.168.2.0/24 via 192.168.1.1``` - to connectr through the route or gateway

```ip route add default via 192.168.2.1``` - this route will be default for all trafic(internet)
default can be represented as 0.0.0.0

Just the commands are good till the next restart - we need to change them in /etc/sysctl.conf

## DNS

