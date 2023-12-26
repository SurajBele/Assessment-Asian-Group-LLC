# Assessment-Test-Asian-Group-LLC
## What is DDoS attacks?
* A distributed denial-of-service (DDoS) attack is a malicious attempt to disrupt the normal traffic of a targeted server, service or network by overwhelming the target or its surrounding infrastructure with a flood of Internet traffic.

## a. CC (Challenge Collapsar) Attack:
---------------------
### Cause:

The CC attack is caused by overwhelming a targeted server with a large number of connections that are seemingly legitimate but are crafted to exploit the server's resources inefficiently.
### Identify:

Identify a CC attack by monitoring the server's connection table. A sudden spike in connections or a rapid increase in the number of connections per second can be indicative of a CC attack.
### Effect:

The effect of a CC attack is a degradation of server performance or a complete denial of service. The server becomes unable to process legitimate requests due to the overload caused by the large number of malicious connections.
### Mitigation:

Mitigate CC attacks by implementing rate limiting or connection rate thresholds. This involves setting limits on the number of connections a single IP address can establish within a specific time frame. Additionally, using web application firewalls (WAFs) can help filter out malicious traffic.

---------------------------------
## b. SYN Flood Attack:
----------------------------
### Cause:

SYN Flood attacks exploit the three-way handshake process in the TCP protocol. Attackers flood a server with a large number of TCP connection requests (SYN packets), but they do not complete the handshake process, leaving the server's resources tied up with incomplete connections.

### Identify:

Identify SYN Flood attacks by monitoring the number of half-open connections. An abnormally high number of half-open connections compared to the normal pattern indicates a SYN Flood attack.

### Effect:

The effect of a SYN Flood attack is the exhaustion of the server's resources, particularly its ability to process new legitimate connection requests. This can lead to service degradation or a complete denial of service.

### Mitigation:

Mitigate SYN Flood attacks by implementing SYN cookies or employing dedicated hardware solutions, such as firewalls or intrusion prevention systems (IPS), capable of identifying and mitigating such attacks. Load balancers can also distribute incoming connections evenly, preventing a single server from being overwhelmed.

----------------------------------
## c. SSL Attack:
--------------------------------
### Cause:

SSL attacks can take various forms, including exploiting vulnerabilities in the SSL/TLS protocols or using resource-intensive cipher suites. These attacks aim to compromise the security of encrypted communication channels.

### Identify:

Identify SSL attacks by monitoring for unusual patterns in encrypted traffic or by detecting anomalies in the SSL/TLS handshake process. Unusual certificate changes or unexpected renegotiations may indicate an SSL attack.

### Effect:

The effect of an SSL attack can range from eavesdropping on encrypted communications to the complete compromise of the confidentiality and integrity of sensitive information.

### Mitigation:

Mitigate SSL attacks by keeping software and systems updated to patch known vulnerabilities. Employing strong encryption algorithms and ciphers, and regularly updating SSL/TLS configurations, helps enhance security. Additionally, using intrusion detection and prevention systems to monitor and block malicious SSL traffic can be effective. Always use reputable SSL certificates and ensure proper certificate management practices are in place. Regular security audits and penetration testing are also recommended.
