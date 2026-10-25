OVERVIEW:

In this wireshark project  using tryhackme date we are going to use the data we have and combine them to understand if there are any activitiesof interest  that may be happening in our network. This seems very fun as it gives us a chance to think critically as an analyst. As it seems to be the capstone of this series, it may be very challenging but it should provide us valuable skills.
 
**PACKET DISSECTION:**

****TASK 1:**Use the "Exercise.pcapng" file to answer the questions. View packet number 38. Which markup language is used under the HTTP protocol?**

I made use of _ctrl g_ which will allow me to enter the packet nuber i want to dissect. this show me the detail of packet 38 which i will be using in this project:

<img width="370" height="272" alt="Image" src="https://github.com/user-attachments/assets/10f35769-26b3-4928-800f-a0de768253d7" />
The langauge uses is **EXTENSIBLE MARKUP LANGUAGE**

**TASK 3:What is the arrival date of the packet? (Answer format: Month/Day/Year)**

In the same packet i look into the hypertext transfer protocol for the date  as shown below:

<img width="372" height="285" alt="Image" src="https://github.com/user-attachments/assets/543e47ba-d695-41f6-8661-bd5d79754114" />

**TASK 3:What is the TTL value?**

The time to live value will be recorded inside the internet trasfer protocol, that is where i found the time to live of the packet:  which is 47.

<img width="368" height="281" alt="Image" src="https://github.com/user-attachments/assets/342b10ee-8323-4570-89a5-cb07d5d5ad10" />

**TASK 4: What is the TCP payload size?**

I foundn the size of the payload will be found in the Transmission comtrol protocol  as shown in the screenshot below: The TCP payload  is 424.

<img width="370" height="278" alt="Image" src="https://github.com/user-attachments/assets/7940b3b1-924d-47c0-9978-e68fa32c9224" />

TASK 5:What is the e-tag value?
The E-TAG Value took me back to the hypertext transfer protocol where i found the e-tag number to be 9a01a-4696-7e354b00  as shown below ;

<img width="372" height="285" alt="Image" src="https://github.com/user-attachments/assets/f5542887-816b-44fc-968a-0f833ce8998e" />

**### PACKET NAVIGATION**

I will be nvigating throght different packet in this project:

**TASK 1:Use the "Exercise.pcapng" file to answer the questions. Search the "r4w" string in packet details. What is the name of artist 1?
I  will be making use of ctlr f bto search for the string:  and i search through the detail pane as shown below the  sting is  r4w8173

<img width="371" height="281" alt="Image" src="https://github.com/user-attachments/assets/99ed7f00-564d-4d2d-9380-a73b8838a05d" />

**TASK 2:Go to packet 12 and read the packet comments. What is the answer?**

Note: use md5sum <filename> terminal command to get MD5 hash
 I press ctrl+g and enter the packet number and we will be directed me to packet 12. Packet 12 directed me to packet 39765. 

<img width="1100" height="558" alt="Image" src="https://github.com/user-attachments/assets/b64d56c2-e011-4c72-8b23-0ddd77ed2f18" />

<img width="161" height="104" alt="Image" src="https://github.com/user-attachments/assets/fae40fbe-ae66-4145-b483-e2e459294de5" />
<img width="368" height="281" alt="Image" src="https://github.com/user-attachments/assets/62f4546a-e240-48f3-8ad5-7f82068d8c93" />

I exported the bytes as shown above then use my terminal to find the has of the image as shwon below:

<img width="270" height="182" alt="Image" src="https://github.com/user-attachments/assets/788ab6bd-9b42-4d6f-a3f4-30977e925edc" />

**TASK 3: There is a ".txt" file inside the capture file. Find the file and read it; what is the alien's name?**

I used another method of exporting objects from a pcap file. i went  to File menu then select Export Objects and then HTTPin thus case  (or whatever protocol that may have been used to transfer objects). Save the “note.txt” file. 

<img width="505" height="491" alt="Image" src="https://github.com/user-attachments/assets/b7159ad4-232b-4627-8f93-2a7a63f7da3f" />

<img width="629" height="462" alt="Image" src="https://github.com/user-attachments/assets/44091c6a-3042-4802-8ce3-a02824687489" />

<img width="500" height="139" alt="Image" src="https://github.com/user-attachments/assets/d324d0a0-7c82-487a-98cc-bbb303413495" />

I read the contents of the text file on the details pane but the objective of this task is for us to learn how to export objects.

<img width="1100" height="844" alt="Image" src="https://github.com/user-attachments/assets/8afb4d49-6ca8-44dc-90a2-34bd2a94e5b5" />

<img width="626" height="533" alt="Image" src="https://github.com/user-attachments/assets/ceda9ea7-4f79-4e56-87bd-ac077a8ece1f" />

The responce o this is **PACKETMASTER**

TASK 4:Look at the expert info section. What is the number of warnings?

I selected  Analyze Menu then choose Expert Information or at the bottom left part of the status bar and click on the first image. we wil find the responce to be 1636

<img width="379" height="289" alt="Image" src="https://github.com/user-attachments/assets/2af6db16-cc6f-4b6b-86cf-1a1ae337d80e" />

<img width="479" height="104" alt="Image" src="https://github.com/user-attachments/assets/59b95081-39f8-4fe7-8727-6f4908ba02ef" />


**### PACKET OPERATION**

**TASK 1:Investigate the resolved addresses. What is the IP address of the hostname starts with "bbc"?**

To achieve this, i need to go to my statistics and click on Resolve address and then typ bbc on the search bar
Thia reveal that the resolve address is **199.232.24.81**

<img width="354" height="289" alt="Image" src="https://github.com/user-attachments/assets/5c0195cf-0345-4aa0-8955-b4eda49f38a1" />

<img width="356" height="282" alt="Image" src="https://github.com/user-attachments/assets/46958f02-db63-419b-ab22-226eaec2cfe8" />

**TASK 2:What is the number of IPv4 conversations?**

In this task, i was able to do this by clicking ion Conversation  and ipv4 to see the number of converstion going on:

<img width="334" height="298" alt="Image" src="https://github.com/user-attachments/assets/17501c41-5de8-4d9c-8e7d-cbc0e714fb64" />

<img width="426" height="276" alt="Image" src="https://github.com/user-attachments/assets/0399a903-617c-429c-8ac9-c9a981d7344a" />

**TASK 3:How many bytes (k) were transferred from the "Micro-St" MAC address?**

I click on the endpoint and look for the "Micro-st" as shown  below:

<img width="446" height="265" alt="Image" src="https://github.com/user-attachments/assets/facf87c7-3da2-4b28-b8d5-9235a278537a" />

**TASK 4:What is the number of IP addresses linked with "Kansas City"?**

i am still on Endpoint on the ipv4 and i loo for Kanscal city in the city column which reveal total of 4

<img width="374" height="188" alt="Image" src="https://github.com/user-attachments/assets/fa01055e-fb89-4383-9291-5442652c1aff" />

TASK 5:Which IP address is linked with "Blicnet" AS Organisation?

 i am still at the Endpoint and ipv4 but this time i search at the Organisation column

<img width="485" height="350" alt="Image" src="https://github.com/user-attachments/assets/85ec5433-459e-4574-a447-8edc4d96f6a0" />

**TASK 6: What is the most used IPv4 destination address?**

To solve this i click on statistics, IPv4 then all Address  whuch reveal to me  IP 10.100.1.33  with  58194

<img width="385" height="300" alt="Image" src="https://github.com/user-attachments/assets/0f560a70-4fee-4c56-bd6d-581b045b07dc" />

<img width="383" height="284" alt="Image" src="https://github.com/user-attachments/assets/39a7aef7-0d32-4403-9949-8e96cbb9eed9" />

**TASK 7:What is the max service request-response time of the DNS packets?**

In this task , i click on statistics, then DNS and it reveal the request-responce time  as 0.467897
s shown below:

<img width="386" height="286" alt="Image" src="https://github.com/user-attachments/assets/fd2ed5ba-afd1-4953-b27a-d30c0472fdf2" />

**TASK 8: What is the number of HTTP Requests accomplished by "rad[.]msn[.]com?**

I clicked on statistics, then Http and all address, i look for the domain "rad[.]msn[.]com" and i scroll to the right side to find the count to be 39.

<img width="376" height="280" alt="Image" src="https://github.com/user-attachments/assets/671a37b5-0bd8-4f52-85fb-fd212f8cf16f" />

**TASK 9: Find all Microsoft IIS servers. What is the number of packets that did not originate from "port 80"?**

In thus task , i made use of the filter below to find the http server with IIS, but doesnt originate from port 80. which return total of 21.

 _http.server contains "IIS" && tcp.srcport != 80_

<img width="353" height="304" alt="Image" src="https://github.com/user-attachments/assets/08a99038-8af0-4809-953e-627216e12c72" />

**TASK 10: Find all Microsoft IIS servers. What is the number of packets that have "version 7.5"?**

In this i  edit the previus filter as follow: 
_http.server contains "IIS" &&  http.server matches "7.5"_

<img width="341" height="298" alt="Image" src="https://github.com/user-attachments/assets/f4d32b68-0262-46a6-b45b-d1fb7026df85" />

**TASK 11:What is the total number of packets that use ports 3333, 4444 or 9999?**

In this task, i made use of the followimg filter to get the total number of packet with Port 3333,4444,9999
http.server matches { 3333 4444 9999}
_tcp.port in {3333 4444 9999}_
The total number display  is **2235**
<img width="336" height="300" alt="Image" src=https://github.com/user-attachments/assets/59640438-21d5-4ffb-bbae-3e6cfd54ae14" />

**TASK 12:What is the number of packets with "even TTL numbers**

In this task i make y=use of the string filter  as follow
string(ip.ttl) matches "{02468}$"
It reveal the total packet to be **77289**

<img width="338" height="290" alt="Image" src="https://github.com/user-attachments/assets/c3f0b5b4-ff03-4a41-9a7b-67608c3b867b" />

**TASK 13: Change the profile to "Checksum Control". What is the number of "Bad TCP Checksum" packets?**

In this task, the first step is to go to edit  and  the configuration policy to change the checksum  

<img width="436" height="290" alt="Image" src="https://github.com/user-attachments/assets/81afc742-5b30-4450-a5a0-e91efb069503" />

After which i make use of the filter below to solve the task above 
_tcp.checksum.status ==0_  as shown inthe screenshot below:
<img width="345" height="304" alt="Image" src="https://github.com/user-attachments/assets/2c41cb94-818b-4d59-b3d9-4fb46ad436dd" />

**TASK 14:Use the existing filtering button to filter the traffic. What is the number of displayed packets?**

at the top right  corner of the previous filter result,  i click in the  checksun control button, and this add rto the filter and reveal  the packets  as **261**
<img width="341" height="300" alt="Image" src="https://github.com/user-attachments/assets/a81d61ee-cfd4-4cf9-8c1f-9051f710b326" />


**### NMAP SCAN**

Task 1:What is the total number of the "TCP Connect" scan.


We will be using the filter and we will type in  this command to search for the total number of tcp connect the

-  “tcp.flags.syn==1 and tcp.flags.ack==0 and tcp.window_size > 1024”
- “tcp.flags.syn==1”   will display all packets with a SYN flag. 
- “tcp.flags.ack==0” will NOT display packets with ACK flag. 
- “tcp.window_size>1024” will display a window size value of greater than 1024._ 

 The result give me the chance to understand what is WINDOW SIZE.  Window size is the the amount of bytes of data the host can send before the receiver will send an acknowledgement. If the host receives an acknowledgement, the window size will increase.  

<img width="367" height="320" alt="Image" src="https://github.com/user-attachments/assets/99fb96b1-8441-4e7b-92f3-d300d8e54f3d" />

As shown the the picture above, The total number of  scan is 1000.

****TASK 2**:How many "UDP close port" messages are there?**

We can make use of these filter :
 **“icmp.type==3 and icmp.code==3”** 
  From the scan  the total number of  udp port is 1083

<img width="369" height="287" alt="Image" src="https://github.com/user-attachments/assets/04bb69de-fd64-406c-877d-f521ea33d2dc" />


****TASK 3:** Which UDP port in the 55-70 port range is open?**

In this task we will be making use of the following filter :
 “udp.port in {55 .. 70}” 
This filter the  udp ports from range 55 to 70. 67 and 69 were attempted but the ports were unreachable. 
ICMP Type = 3 and ICMP Code = 3, indicating closed ports.The only one that’s open is port 67

<img width="357" height="252" alt="Image" src="https://github.com/user-attachments/assets/96d56c3f-7ded-46cf-b1ff-86fb48364bd8" />

##**### #  **ARP Poisoning/Spoofing (A.K.A. Man In The Middle Attack)*

ARP (Address Resolution Protocol) helps devices map IP addresses to MAC addresses on a local network.
ARP Poisoning, also called ARP Spoofing or a MITM attack, occurs when an attacker sends malicious ARP packets to manipulate the network's IP-to-MAC address table. This can allow the attacker to intercept and sniff the target's network traffic.

****TASK 1:** What is the number of ARP requests crafted by the attacker?**

My first step in this task is to find out the IP address  and MAC address is since it seem ,ike the attacker will be scaniing the system.To find out i makd use of the filter bellow
 _arp.dst.hw_mac==00:00:00:00:00:00_

<img width="370" height="323" alt="Image" src="https://github.com/user-attachments/assets/3353843f-4511-4ba9-83ce-0871da396295" />
As shown above the scan reveal the source MAC address to be _"00:0c:29:e2:18:b4 "_ then i have to filter making use of this MAC address an specifying for only request by adding the filter below:

_**_&& (eth.src == 00:0c:29:e2:18:b4) && (arp.opcode==1)_
breakdown:
&& (eth.src == 00:0c:29:e2:18:b4) search for the source MAC address
&& (arp.opcode==1) and search for the request only:**_
{full command:(eth.src == 00:0c:29:e2:18:b4) && (eth.src == 00:0c:29:e2:18:b4) && (arp.opcode==1)}

<img width="387" height="329" alt="Image" src="https://github.com/user-attachments/assets/f443fd67-5737-4edb-b394-7d0331c02e56" />

This confirm the total number of request by the attcker to be **"284"**

****TASK 2:** What is the number of HTTP packets received by the attacker?**

From the task above, i have been able to discover what the MAC address of the attacker is. This information will be helpfull in this task: We make us of the filter below  which indicate the MAC address and the http
_eth.addr == 00:0c:29:e2:18:b4 && http_

<img width="387" height="329" alt="Image" src="https://github.com/user-attachments/assets/fdcccbf9-64f3-4649-a2df-1b8920a0f6a1" />
As show in the screenshot above the  number of HTTP packets received by the attacker i**s 90.**

****TASK 3**: What is the number of sniffed username&password entries?**
From the previous task, the scan reveal an interesting frame. Inside this frame we see POST and /userinfo.php

<img width="370" height="310" alt="Image" src="https://github.com/user-attachments/assets/5bfe2775-c4d5-42a1-b1f1-1b6e3812f2ce" />

 I then click on the drop-down carot on Hypertext Transfer Protocol. Again click on the drop-down carot next to POST /userinfo.php. You should now see Request URI: /userinfo.php. Right-click on Request URI: /userinfo.php, from the drop-down menu hover your cursor over **Apply as Filter**. When the new drop-down menu appears, move your cursor over to …**and Selected.** Then click on it.
As shown below
<img width="394" height="304" alt="Image" src="https://github.com/user-attachments/assets/b726f04c-fa4b-4fc7-8b88-cc5da683a494" />

This will reveal that we have 8 packet left  in which 2 of them are bit bigger. I clicked on one of those and click on the html form to reveal the username  but no password while the remaining 6 shown both the username and passwords;

<img width="328" height="200" alt="Image" src="https://github.com/user-attachments/assets/9c1d706a-8edb-4d5c-97f0-d17ec8350cbf" />

<img width="359" height="293" alt="Image" src="https://github.com/user-attachments/assets/b02841b9-682c-41c1-8e37-29b87370428f" />

I remove the 2 big packet without the password and we have 6 packet that has got password revealed: which reveal  the number of sniffed username&password entries to be **6.**



**TASK 4: What is the password of the "Client986"?**|

In this task i need to click on all the remaining 6 packet to search for client986 .

<img width="342" height="201" alt="Image" src="https://github.com/user-attachments/assets/6bc2b005-6453-4844-9734-0465e0d8dbeb" />

**TASK 5:What is the comment provided by the "Client354"?**

i adjust my filter a bit by deleting the "HTTP URI of /userinfo.php" ffrom the filter. i then  right-click on HTML Form URL Encoded: application/x-www-for-urlencoded. On the drop-down menu, then  Apply as Filter. Then an new drop-down will appear, click on …and Selected.This gave us addition 2 new packet for our search. 

<img width="335" height="218" alt="Image" src="https://github.com/user-attachments/assets/e3e5d395-4a1c-4fe6-b115-d2d8a0d60480" />
Seaching through the 2 new packet ,i found  the  comment to be "nice work! as found in the attached screenshot

<img width="322" height="202" alt="Image" src="https://github.com/user-attachments/assets/5fe1739e-5ce8-428e-9057-6fbc71414a6b" />

### **DHCP, NETBIOS AND KERBEROS**
In this project i will be analysing traffic based on DHCP,NetBios and Kerberos:

Task 1:What is the MAC address of the host "Galaxy A30"?
I use the filter below to search for packt with host name cotains Galavy 
_dhcp.option.hostname contains "Galaxy"_

<img width="398" height="312" alt="Image" src="https://github.com/user-attachments/assets/3d5f2d64-9935-4f9b-93a1-0c5ea61361d8" />
This reveal the Mac Address to be 9a:81:41:cb:96:6c

**TASK 2:How many NetBIOS registration requests does the "LIVALJM" workstation have?**

I created a query using the Display Filter Expression. The first one is building an NBNS registration request filter, and the second one is filtering NBNS names that match only the workstation “LIVALJM”

<img width="368" height="296" alt="Image" src="https://github.com/user-attachments/assets/cf3f9add-ddcf-4d0d-8cea-e7326a86b1cf" />

<img width="362" height="308" alt="Image" src="https://github.com/user-attachments/assets/c81a4487-e670-4cfa-9b0d-fe15d0fedc68" />

<img width="359" height="299" alt="Image" src="https://github.com/user-attachments/assets/2d7bfe67-c3ff-469b-b268-1a3107170d61" />

it display  as 16.

**TASK 3: Which host requested the IP address "172.16.13.85"?**
In this  task i make use of the filter below to serch for the ip  in the question:

_dhcp.option.dhcp == 3 && dhcp.option.requested_ip_address == 172.16.13.85_

This reveal the  host name to be Galaxy A12 as shown below:

<img width="362" height="281" alt="Image" src="https://github.com/user-attachments/assets/173508ab-57b3-4f6e-ac14-7b0709983799" />

**Task 4: What is the IP address of the user "u5"? (Enter the address in defanged format.)**
I made use of the filter below to search for the packet of ip address of the user
 _kerberos.CNameString contains "u5"_
This reveal the ip address to be  10.1.12.2 . I then make use of Cyberchef to convert this to defanged format:

<img width="358" height="318" alt="Image" src="https://github.com/user-attachments/assets/bedf105a-89a5-4514-a9d7-fee12c07c8e8" />

<img width="852" height="279" alt="Image" src="https://github.com/user-attachments/assets/eb219ba1-74eb-4dcb-b0b2-db94e44708f8" />

The defanged Ip Address is 10[.]1[.]12[.]2
 
TASK  5: What is the hostname of the available host in the Kerberos packets?
I made use of the filter below to search for Values that end with “$” are hostnames, and the ones without it are usernames.
_kerberos.CNameString contains "$"_

<img width="359" height="281" alt="Image" src="https://github.com/user-attachments/assets/634eb4b3-f184-4bd3-b18c-c3e572aa0fb8" />

**Tunnelling Traffic: ICMP and DNS**
Internet Control Message Protocol (ICMP) is designed for diagnosing and reporting network communication issues. it is used by the aderversary  for denial of service (DoS) attacks; data exfiltration and C2 tunnelling activities.
Domain Name System (DNS) is designed to translate/convert IP domain addresses to IP addresses. It is also known as a phonebook of the internet. As it is the essential part of web services, it is commonly used and trusted, and therefore often ignored. Due to that, adversaries use it in data exfiltration and C2 activities.

**TASK 1:Use the "Desktop/exercise-pcaps/dns-icmp/icmp-tunnel.pcap" file. Investigate the anomalous packets. Which protocol is used in ICMP tunnelling?**
I made use of the below filter to  filter for packet with data byte is greater than 40, as the bigger the byte the chance of maliscious activities going on:
_data.len > 64 and icmp_ 

<img width="365" height="292" alt="Image" src="https://github.com/user-attachments/assets/a8f656b1-c131-45e7-bf51-d19d1db83839" />
 
As shown above, the filter did not giev enough data to analise, So we will modify the query to include the protocols commonly used for data exfiltration such as SSH, FTP, TCP, and HTTP.

_(data.len > 64) and (icmp contains "ssh" or icmp contains "ftp" or icmp contains "tcp" or icmp contains "http")_

<img width="370" height="297" alt="Image" src="https://github.com/user-attachments/assets/6982ba81-2c48-4c38-8e87-8398ad3f8170" />
This shownthat the  protocol is "ssh"

**TASK 2:Use the "Desktop/exercise-pcaps/dns-icmp/dns.pcap" file.Investigate the anomalous packets. What is the suspicious main domain address that receives anomalous DNS queries? (Enter the address in defanged format.)**
For this task, i made use of the filter below to attain the result
_dns.qry.name.len > 40 and !mdns_ 

<img width="492" height="404" alt="Image" src="https://github.com/user-attachments/assets/de6323c3-f1ae-4d79-a1d7-9ca4fd6b47dc" />

As shown above, the  suspiscious domain address is _"dataexfil[.]com"_


**### FTP Analysis**
Ftp has some series which we will be making use of in this task suche as the x1x, x2x, x3x series with their respective code.
with the global search as: _ftp.request.code == "code"_ s listed below:

**"x1x" 
211: System status.
212: Directory status.
213: File status

x2x" series options for grabbing the low-hanging fruits:
220: Service ready.
227: Entering passive mode.
228: Long passive mode.
229: Extended passive mode

"x3x" series options for grabbing the low-hanging fruits:
230: User login.
231: User logout.
331: Valid username.
430: Invalid username or password
530: No login, invalid password.**

**TASK 1: How many incorrect login attempts are there?**

I  make use of the filter below to  query for all failed logging attempt:
_ftp.response.code == 530_
which disply the total incorect login attempt to be 737

<img width="356" height="304" alt="Image" src="https://github.com/user-attachments/assets/8e3dd58b-ceef-4843-95cd-8fc6e4e41668" />

TASK 2:What is the size of the file accessed by the "ftp" account?
I make use of  the query below to get the file status 
ftp.response.code == 213

<img width="356" height="292" alt="Image" src="https://github.com/user-attachments/assets/f30d2bb0-ccf4-45ba-9741-ddfc1899a2ad" />
 This reveal the result to be **39424**

**### HTTP Analysis**

Just like ftp, Http has a request method and the responce code too the request  method such as GET, POST and REQUEST. With the respobnd code depending on the response return from the server:

**200 OK: Request successful.
301 Moved Permanently: Resource is moved to a new URL/path (permanently).
302 Moved Temporarily: Resource is moved to a new URL/path (temporarily).
400 Bad Request: Server didn't understand the request.
401 Unauthorised: URL needs authorisation (login, etc.).
403 Forbidden: No access to the requested URL. 
404 Not Found: Server can't find the requested URL.
405 Method Not Allowed: Used method is not suitable or blocked.
408 Request Timeout:  Request look longer than server wait time.
500 Internal Server Error: Request not completed, unexpected error.
503 Service Unavailable: Request not completed server or service is down.**

TASK 1:Investigate the user agents. What is the number of anomalous  "user-agent" types?
To resolve this, i put the query _http.user_agent_ in the search bar, search through te packet to fine the user agent and  apply the user agent as a column

<img width="355" height="286" alt="Image" src="https://github.com/user-attachments/assets/78736b67-cd65-4421-9eee-27583a3e2c9d" />
<img width="482" height="355" alt="Image" src="https://github.com/user-attachments/assets/12ddd4eb-4e6a-437c-aef0-cdd227e35468" />
 as ahown above the  number of anomalous packet is **6.**

**TASK 2: What is the packet number with a subtle spelling difference in the user agent field?**
I with the same quesry i looked for  packet in which the user agwtn feild is mispelled which appear on packet 52.

<img width="465" height="173" alt="Image" src="https://github.com/user-attachments/assets/dcfacd40-c524-4ff0-b3e8-053d54161055" />

**TASK 3: Locate the "Log4j" attack starting phase. What is the packet number?**
In this task , i make use of the query below o acheice the  packet number
 _(http.user_agent contains "$") or (http.user_agent contains "==")_

<img width="397" height="113" alt="Image" src="https://github.com/user-attachments/assets/584299b1-f156-4e3f-98cd-fa7790d3fafc" />

**TASK 4:Locate the "Log4j" attack starting phase and decode the base64 command. What is the IP address contacted by the adversary? (Enter the address in defanged format and exclude "{}".)**
 I Copy the value of the User-Agent then decode it from base 64 using cyberchef.

<img width="369" height="314" alt="Image" src="https://github.com/user-attachments/assets/4b91a494-a48c-400e-898e-8039cf046c07" />

<img width="1013" height="284" alt="Image" src="https://github.com/user-attachments/assets/5918195b-fbf3-4376-a867-88ae6c9d92b0" />

The defange Ip address is  : 62[.]210[.]130[.]250

 
**### Decrypting HTTPS Traffic**
Hypertext Transfer Protocol Secure (HTTPS) protocol for enhanced security against spoofing, sniffing and intercepting attacks. HTTPS uses TLS protocol to encrypt communications, so it is impossible to decrypt the traffic and view the transferred data without having the encryption/decryption key pairs. As this protocol provides a good level of security for transmitting sensitive data, attackers and malicious websites also use HTTPS. Therefore, a security analyst should know how to use key files to decrypt encrypted traffic and investigate the traffic activity.
Since http make use of Tls for encryption they follow the 3 way handshake of 
Client request == 1
Server response == 2

**TASK 1:What is the frame number of the "Client Hello" message sent to "accounts.google.com"?**

During this task, i made use of the following query to filter all packet with of client request OR tls handshake type 
is equal to 1 (request)  and its not an SSDP request (SSDP is a network protocol that provides advertisement and discovery of network services.)The query i as follow:

_(http.request or tls.hanshake.type ==1 )  and !(ssdp)_

<img width="479" height="365" alt="Image" src="https://github.com/user-attachments/assets/6c4936b3-9191-439f-a3ce-f94d3bd7e34d" />
This reveal the packet number 16 to be the packet.

**TASK 2: Decrypt the traffic with the "KeysLogFile.txt" file. What is the number of HTTP2 packets?**
In this task i aAdded the key log file: “Edit → Preferences → Protocols → TLS” menu. Then filter only http2 packets.

<img width="735" height="501" alt="Image" src="https://github.com/user-attachments/assets/e32015b8-8cec-4a62-b866-29ebaa0941bb" />

With the query of http2 it returned a total of 115 packet.

<img width="370" height="293" alt="Image" src="https://github.com/user-attachments/assets/210fe4f3-4f21-4ad4-990b-f387d7432d6b" />

TASK 3: Go to Frame 322. What is the authority header of the HTTP2 packet? (Enter the address in defanged format.)
I make use of ctrl+g and go to packet 322. then click on thhe header to have search for the authority header 

<img width="358" height="284" alt="Image" src="https://github.com/user-attachments/assets/272c3ab1-c253-4fe7-8ccd-1bf24545e018" />
I found the header nand i defange it with CYBERCHEF. 

safebrowsing[.]googleapis[.]com


In this project , i made use of the Tools section where i can see all packet with clear text accoring to their protocols, and packet numbers:

<img width="439" height="239" alt="Image" src="https://github.com/user-attachments/assets/dcfe655b-6e6c-4cd9-9b9e-e3192d824e0d" />
<img width="320" height="251" alt="Image" src="https://github.com/user-attachments/assets/2782d84c-5a64-4d5e-9ddc-a46a575a028d" />

In addition from the tool section i was able to set a ip firewall rule to block and allow traffic on a packet as shown in the screenshot below:

<img width="467" height="383" alt="Image" src="https://github.com/user-attachments/assets/28b9a4b2-83a6-4c17-88ec-8d7aa898f0fc" />
<img width="347" height="254" alt="Image" src="https://github.com/user-attachments/assets/d9602af4-c5c1-4ece-a2fc-5d9a4027678d" />

**CONCLUSION :Wireshark is a good tool for starting a network security investigation. However, it is not enough to stop the threats.** 
