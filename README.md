# Testing NIDS in a maritime environment 

## Summary
This project examines the effectiveness of Network Intrusion Detection Systems (NIDS) in detecting NMEA spoofed messages in a stimulated maritime environment. 

## Objective
To investigate how NIDS tools, such as Snort, Suricata, and Wazuh, detect spoofing attacks in maritime navigation systems.

## Lab setup
• Ubuntu Desktop (NIDS host)
• Monitoring Laptop (Stored Spoofing script and Wireshark for monitoring)
• Panasonic Toughbook (Stored & replayed original pcap.files,)
• Network switch (shared domain)

## Tools 
• Suricata
• Snort 3
• Wazuh
• Wireshark
• Tcpdump
• Python (spoofing script)

## Attack Simulation
• Spoofed NMEA messages injected via Python script
• UPD traffic monitored by NIDS
• Analyse and differentiate between real and spoofed traffic

## Detection Method
• Tailored rules for anomaly detection
• Abnormal spikes in coordinates
• NMEA sentence patterns such as $GPGGA, $GPRMC
• Deformed identifiers

## Results
• 86% detection rate of spoofed messages
• Suricata performed best and was able to detect spoofed messages in the network traffic.
• Snort 3 required advanced rule tuning to be able to detect.
• Wazuh showed potential but required a better integration.

## Scrrenshots














## Conclusion
NIDS can help mitigate spoofed messages in network traffic, but its effectiveness depends on correct configurations, the integration of appropriate tools, and tailored rules for detection.
