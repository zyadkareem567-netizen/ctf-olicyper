# URL
* https://training.olicyber.it/challenges#challenge-238
# concept
* ```network forensics challenge```
# method of solving 
* in this challenge there are a pcap file you should analyze it using wireshark and the flag for this challenge you will found in the tcp file .
* first you should install the wireshark tool ```sudo apt install wireshark``` and this is the code to install it .
* then to read the networks that working in the pcap file ```tshark -r nw-intro01.pcap```
* then the next step use this command the flag will appear with you ```tshark -r file.pcap -Y "tcp.len > 0" -x```
* the flag ```flag{Y0u_kn0w_Wh4t_a_Pc4p_1s}```
