# txlf2026
Texas LinuxFest 2026

See the contents of my github repo at https://github.com/tdcam/txlf2026

The network configuration is in the slide deck at:
https://people.redhat.com/tcameron

First, the network setup. I tried to emulate an enterprise network setup.
I have a public/enterprise network 172.31.100.0/24. That's where the consumers
of apps on OKD will be coming from. I am running the OKD cluster on a private
network 10.31.100.0/24. It is behind a load balancer running haproxy on a 
CentOS Stream 10 machine. 

Get DNS set up. In my lab, I have the example.com domain. I created a
second domain called okd.example.com for all the OKD hostnames. I do this so
I can enable or disable the okd.example.com domain as needed without having to
add a bunch of weird entries to the example.com zone file. 

Next, set up 
