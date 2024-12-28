Networking Commands

# ifconfig - gives us the information about network devices.

To get ipv4 Address 

# ip -4 addr

To get ipv6 address:

# op -6 addr

#netstat - detailed network activity on the linux machine
# netstat -a -> gives all of the listening ports over tcp/udp connections.
# netstat -at - shows all the tcp connections.
# netstat -u - shows all the udp connections.
# netstat -l -> gives all the active ports.


# curl ->   to test an endpoint or can be used to get data from an endpoint.

# curl https://google.com

To send Post or put methods for an endpoint.

# curl -X POST --data "p1=v1 & p2=v2" http://mountblue.in
# curl -X POST  -d param1=v1 -d param2=v2 http://mb.in

To save output from an endpoint to a file,we use 

# curl -o outputFile http://mountblue.in

To get the http header from the response (ex : 200,404, 503)
# curl -I http://mb.in


# ping  (ping google.com)

This command will send data packets to an endpoint continuously to check whether we receive response or not.