# siri
from scapy.all import* def packet_callback(packet): print(packet.summary()) if packet.haslayer(IP): print("source IP:",packet[IP].src) print("destination IP:",packet[IP].dst) print("protocol:",packet[IP].proto) print("_"*50
