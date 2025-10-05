# URL
* https://training.olicyber.it/challenges#challenge-239
# CONCEPT
* network hacking

# METHOD OF SOLVING
* this challenge needs ```the mac address``` and ```data bytes length```
* and you get them from the line 4 in the file in the challenge 
* you will get them with this code ```tshark -r nw-intro02.pcap -Y "tcp.len > 4" -T fields -e eth.src -e tcp.len```
* and this what you will get ```26:0e:ad:ef:c6:65  63```
* the mac address is the first part then after the back slash the data bytes length 
* then the flag will be ```flag{26:0e:ad:ef:c6:65/63}``` like this 
* the meaning of this code 

```-r file.pcap```
-r = Read from file
file.pcap = The capture file you want to analyze
Instead of capturing live traffic, read from an existing file

```-Y "tcp.len > 0"```

-Y = Display filter (same filters as Wireshark GUI)
"tcp.len > 0" = Only show TCP packets where data length is greater than 0
This filters OUT empty packets (handshake SYN, ACK with no data)
Only shows packets that actually contain payload/data

```-T fields```

-T = Output format type
fields = Output only specific fields (not full packet details)
Makes output clean and easy to read (just the values you want)

```-e eth.src```

-e = Extract/display this field
eth.src = Ethernet source address (source MAC address)
Shows which device sent the packet

```-e tcp.len```

-e = Extract/display this field
tcp.len = TCP data length (size of payload in bytes)
Shows how much actual data is in the TCP packet**
