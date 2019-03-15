- Any encryption applied to wireless networks only encrypts the data itself, leaving the header potion of the wireless frame open to many types of attacks

- Understanding the 802.11 standards and protocols

- 802.11 Wireless Lans operates at layer 1 and 2 (Physical and data level)

- 802.11 frame formats have a different format than 802.3 (Ethernet)
    - Ethernet Layer 2 frames carry only two MAC addresses, while 802.11 frames have fields for four MAC addresses
    - Ethernet just defines source and destination addresses
    - 802.11 frame can define source, destination, transmitter and receiver
    - 802.11 frames also carry a frame control field in the MAC header used to indicate information about the frame, such as if the frame is encrypted
    
- Layers 3 and above, the operations and formats are similar to ethernet

- 3 types of 802.11 frames
    - Management: Used for notification, connection, disconnection, and information
    - Control: Used to control which station has access to the wireless network media
    - Data: Used to carry upper layer data
   
- Most wireless lans area based off different standards and ammendments
    - 802.11a, 802.11b, 802.11g, and 802.11n
    - Standard / Freq / Speed / Transmission Range / Spread Specturm
    - 802.11 / 2.4 GHz / Up to 2 Mbps / Depends on spread spectrum type / DSSS and FHSS
    - 802.11a / 5 GHz / Up to 54 Mbps / 25 to 75 feet indoors; range can be affected by building materials / OFDM
    - 802.11b / 2.4 GHz / Up to 11 Mbps / Up to 150 feet indoors; range can  be affected by building materials / DSSS
    - 802.11g / 2.4 GHz / Up to 54 Mbps / Up to 150 feet indoors; range can  be affected by building materials / DSSS
    - 802.11n / 2.4 and 5 GHz / Up to 600 Mbps / At least as far as b, g, and a—and possibly much further / OFDM
    
- Authentication and Cracking Techniques

- Two methods exist in the 802.11 standard for authenticating wireless LAN clients to an access point
    - Open system
        - Does not provide any security mechanisms but is simply a request to make a connection to the network
    - Shared-key authentication
        - Client hashes a string of challenge text with the Wired Equivalent Privacy (WEP) key to authenticate the client to the network
        
- WEP is used to encrypt data on the WLAN and can optionally be paired with shared-key authentication to authenticate WLAN clients
    
- WEP Security
    - Wi-Fi Security / Authentication / Cipher / Encryption
    - WPA-Personal / Preshared Key / TKIP / RC4
    - WPA-Enterprise / 802.1X or EAP / TKIP / RC4
    - WPA2-Personal / Preshared Key / CCMP (default), TKIP (optional) / AES (default), RC4 (optional)
    - WPA2-Enterprise / 802.1X or EAP / CCMP (default), TKIP (optional) / AES (default), RC4 (optional)

- WPA2 Personal uses passphrase

- WPA2 Enterprise uses RADIUS

- 802.11i and WPA use the same encryption and authentication mechanisms as WPA2
    - However, WPA2 doesn’t require vendors to implement preauthorization
    - Preauthorization enables fast, secure roaming, which is necessary in very mobile environments with time-sensitive applications such as wireless VoIP
    
- Packets are generally sent unencrypted across the WLAN

- Passwords for network access protocols such as FTP, POP3, and SMTP can be captured in cleartext (unencrypted) by a hacker on an unencrypted WLAN
 
- Service Set Identifier (SSID) is the name of the WLAN and can be located in beacon frames and probe response frames
    - The SSID is usually sent in the clear in a beacon frame as well as other frames, such as probe response frames
    - Most APs allow the WLAN administrator to hide the SSID
    - However, this isn’t a robust security mechanism because some tools can read the SSID from other packets, such as probe requests and other client-side packets

- Early security solution in WLAN technology used MAC address filters
    - List of valid MAC addresses for the systems allowed to associate with the AP
    - MAC filters are cumbersome to configure and aren’t scalable for an enterprise network because they must be configured on each AP
    
- MAC spoofing can defeat MAC address filters, and MAC headers are never encrypted in your wireless packets

- Rouge Access Points
    - Rogue access points are WLAN access points that aren’t authorized to connect to a network
    - The resulting rogue AP can be used by anyone who can connect to the AP, including a hacker, giving them access to the wired LAN
    - Organizations that have a “no wireless” policy need to perform wireless scanning to ensure no rogue APs are connected to the network
 
 - Evil Twin / AP Masquerading
     - An AP that looks like the real AP
     
 - Wireless Hacking Techniques
     - Cracking Encryption
     - Eavesdropping / Sniffing
     - DoS
     - Evil Twin
     - MAC spoofing
     - Rouge AP
 
- Securing Wireless Connections
    - Change default settings
    - WEP/WPA encryption
    - Change default SSID
    - Don't auto connect to open WIFI
    - Enable Firewall
    - Reduce WLAN transmitting power
    - Disable remote administration
    
# Essentials

- Understand vulnerabilities of using WLAN

- Security solutions in 802.11 standard

- WPA, WPA2

- SSID in WLAN

- WEP and MAC filters should not be the sole security for WLAN
    
# Exam Notes

- WEP uses same key for encryption and authentication

- VPN is a layer 3 security solution for WLAN

- 802.11 is a layer 2 security

- WPA personal for home. WPA Enterprise should  not be used for home because it uses a RADIUS server, which will not be present in homes

 
  
  
  
    
