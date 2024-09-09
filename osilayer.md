# From Physical to Application: Understanding the OSI Layers in Cyber Security
###### _Ahsen Beyza Özkul_
<ahsenbeyzaozkul@gmail.com>

## Introduction
Understanding how information travels through computer networks can seem complicated, but the Open Systems Interconnection (OSI) Model makes it more manageable. Developed in 1984 by the International Organization for Standardization (ISO), this model breaks down network communication into seven distinct layers, each with a specific role.

Think of the OSI Model as a stack of layers where each one handles a different aspect of data transmission. This approach simplifies the understanding of network processes, helps in troubleshooting issues, designing networks, and securing data. Although today we often use the TCP/IP model, the OSI Model remains a valuable tool for visualizing and addressing network challenges.

In the following sections, this paper will into each layer of the OSI Model, offering clear explanations, simple examples, and tips for securing each layer. The goal is to make the OSI Model easier to understand and apply in practical network and security scenarios.

## What is the OSI Model?

The Open Systems Interconnection (OSI) model is a way to understand and describe how different parts of a computer network work together to enable communication. Think of it like a set of layers, each with its own specific job, stacked on top of one another. This helps to break down complex networking processes into simpler, more manageable pieces.

In more straight forward words,the OSI Model is a conceptual framework used to understand how different parts of a computer network work together to facilitate communication. Introduced in 1984 by the International Organization for Standardization (ISO), this model provides a structured approach to networking, breaking down the complex process into seven distinct layers. Although modern networks mostly use the simpler TCP/IP model, the OSI Model remains relevant because it offers a clear way to visualize and troubleshoot network issues.


## Why is the OSI Model Important?

1.	Standardized Communication: Think of the OSI model as a common language that helps different devices and programs talk to each other. Just like how you can speak English with people from different places, devices and software use the OSI model to understand each other, even if they’re from different companies.
2.	Easier Troubleshooting: If there’s a problem with your network—like if you can’t connect to the internet—the OSI model helps you figure out where the problem is. It’s like having a map to find out which part of a complex system is not working. You can check each layer to see where things are going wrong.
3.	Helping with Product Design: For companies making networking equipment or software, the OSI model helps them design their products. They can say, “Our product works at Layer 4” (which is about managing connections) so you know exactly what it does. This makes it easier to choose the right products for your needs.
4.	Guiding Software Development: Developers use the OSI model when they create new applications. It helps them know which part of the communication process their app will handle, so they can make sure it works well with other apps and devices.
5.	Improving Security: The OSI model also helps keep data safe. By understanding which layer handles different types of data, security experts can put the right protections in place to keep your information secure.
6.	Long-Term Use: Even though there are newer technologies, the OSI model is still useful. It provides a clear way to understand and compare different network systems and helps ensure that everything works together smoothly.

Understanding the OSI model helps you grasp how different network components and protocols work together. It’s useful for troubleshooting network issues, designing networks, and ensuring that various technologies can work together. 
Even though the OSI model is more of a theoretical framework, knowing it helps you understand and manage real-world networking scenarios and security considerations.

By breaking down each layer and understanding its role, you can see how data moves through a network and how different protocols and devices interact. This foundational knowledge is crucial for anyone working with or learning about networks.



## Layers of OSI

1)	Layer 7: Application Layer

   - What It Does: This is the layer closest to the end user. It’s where all the applications and services that you interact with live. It’s responsible for providing network services to applications, like web browsers and email clients.

   - Simple Example: When you use a web browser to visit a website, the Application Layer handles your request and displays the website on your screen. It uses protocols like HTTP (HyperText Transfer Protocol) to communicate with web servers.

2)	Layer 6: Presentation Layer

   - What It Does: The Presentation Layer is responsible for translating data from the Application Layer into a format that can be understood by the network and vice versa. It also handles data encryption and compression.

   - Simple Example: If you’re sending an encrypted email, the Presentation Layer encrypts the email before it’s sent. When the recipient gets it, this layer decrypts it so they can read the message. It also makes sure the data is in a format that the Application Layer can work with.

3)	Layer 5: Session Layer

   - What It Does: This layer manages and controls the connections between computers. It sets up, maintains, and ends communication sessions between applications on different devices. It also handles the flow of data and any interruptions in communication.

   - Simple Example: During a video call, the Session Layer ensures that the connection between your computer and your friend's computer remains active and properly organized. It manages the session so that the call doesn’t drop and keeps everything synchronized.



4)	Layer 4: Transport Layer

   - What It Does: The Transport Layer ensures that data is transferred reliably and in the correct order between devices. It breaks down data into smaller packets, manages error-checking, and controls the flow of data.

   - Simple Example: When you download a file from the internet, the Transport Layer splits the file into smaller packets, sends them to your computer, and then reassembles them in the correct order. It also checks for errors in transmission and requests retransmission if needed. Two key protocols at this layer are TCP (Transmission Control Protocol), which focuses on reliable delivery, and UDP (User Datagram Protocol), which is faster but less reliable.

5)	Layer 3: Network Layer

   - What It Does: This layer handles the routing of data across different networks. It determines the best path for data to travel from the source to the destination and adds addressing information to the data packets.

   - Simple Example: When you send an email from your computer to a friend’s computer on a different network, the Network Layer decides how to get the email across the internet. It adds an IP (Internet Protocol) address to the email so that it reaches the correct destination. Routers at this layer help direct the email along the best path.

6)	Layer 2: Data Link Layer

   - What It Does: The Data Link Layer ensures that data is correctly transferred over a local network. It handles error detection and correction, and manages the flow of data between devices on the same network.

   - Simple Example: When you send a file over your home Wi-Fi, the Data Link Layer makes sure the file is sent to the correct device within your local network. It adds MAC (Media Access Control) addresses to the data packets and organizes the data for transmission over the physical network medium, like cables or wireless signals.

7)	Layer 1: Physical Layer

   - What It Does: This is the lowest layer and deals with the physical connection between devices. It involves the hardware and the physical means of transmitting data, such as cables, switches, and network cards.

   - Simple Example: The Physical Layer includes things like Ethernet cables, Wi-Fi signals, and the actual hardware (like network cards) that transmit data. It’s responsible for converting data into electrical signals or light pulses that travel through the cables or air.


## Mnemonics to Remember the Layers

To help remember the layers and their order, we can use these mnemonic phrases:

* From Top to Bottom (Layer 7 to Layer 1): "All People Seek To Need Data Processing" (Application, Presentation, Session, Transport, Network, Data Link, Physical)
* From Bottom to Top (Layer 1 to Layer 7): "Please Don’t Nick The Sausage Pizza Away" (Physical, Data Link, Network, Transport, Session, Presentation, Application)


## Security in the OSI Model and On 7 Layers

1.	Physical Layer (Layer 1): 
Handles the transmission of raw bits over physical media, such as cables and switches.

Security Vulnerabilities:

   - Eavesdropping: Attackers can tap into cables or intercept wireless signals to capture data.
   - Physical Attacks: Sabotage, theft, or vandalism can disrupt network operations.

Security Measures:

   - Physical Security: Use access controls, surveillance cameras, and biometric authentication to secure data centers and network equipment.
   - Secure Cabling: Implement cabling practices that prevent tampering and eavesdropping.
   - Hardware Security Modules (HSMs): Protect cryptographic keys and perform secure operations to prevent unauthorized access.

2.	Data Link Layer (Layer 2): 
Manages communication between devices on the same network segment and handles error detection and correction.

Security Vulnerabilities:

   - MAC Address Spoofing: Attackers can impersonate legitimate devices by changing their MAC addresses.
   - Switching Attacks: Malicious users can exploit switches to intercept traffic or launch attacks.


Security Measures:

   - MAC Address Filtering and Port Security: Restrict access to network devices based on MAC addresses and control access to switch ports.
   - VLANs (Virtual Local Area Networks): Segment network traffic to isolate sensitive data and devices.
   - Ethernet Encryption: Use protocols like MACsec to encrypt data transmitted between devices.

3.	Network Layer (Layer 3): 
Routes packets across multiple networks and determines the best path for data transmission.

Security Vulnerabilities:

   - IP Spoofing: Attackers forge IP addresses to bypass security measures or launch attacks.
   - Routing Attacks: Manipulation of routing tables can lead to traffic interception or redirection.

Security Measures:

   - Firewalls: Filter and control traffic based on IP addresses, ports, and protocols.
   - VPNs (Virtual Private Networks): Create secure, encrypted tunnels over public networks.
   - Intrusion Detection and Prevention Systems (IDS/IPS): Detect and block malicious network activities.

4.	Transport Layer (Layer 4): 
Ensures reliable data transmission and manages error correction and flow control.

Security Vulnerabilities:

   - Man-in-the-Middle Attacks: Attackers intercept and modify data between communicating parties.
   - Denial-of-Service (DoS) Attacks: Overwhelm a server with excessive requests, disrupting service.

Security Measures:

   - TLS/SSL Encryption: Secure data in transit between client and server applications. Consider aspects like backward compatibility and Perfect Forward Secrecy.
   - Firewall Rules and ACLs: Restrict access to specific ports and services.
   - Session Management: Use secure techniques like session tokens and secure cookies to prevent session hijacking.

5.	Session Layer (Layer 5): 
Manages sessions or connections between applications, including session establishment, maintenance, and termination.

Security Vulnerabilities:

   - Session Hijacking: Attackers take control of an active session or monitor network traffic to steal session tokens.

Security Measures:

   - Session Encryption and Integrity: Secure communication sessions using encryption.
   - Session Management Protocols: Implement protocols like OAuth and OpenID Connect for secure authentication and authorization.
   - Session Timeout Policies: Automatically terminate inactive sessions to mitigate session fixation attacks.

6.	Presentation Layer (Layer 6): 
Translates data formats between the application layer and the network, including data encoding, encryption, and compression.

Security Vulnerabilities:

   - Data Exposure: Unencrypted or poorly encoded data can be intercepted or tampered with.

Security Measures:

   - Data Encoding and Encryption: Use techniques like Base64 encoding and AES-256 encryption to protect data.
   - Secure Data Serialization: Utilize formats like JSON Web Tokens (JWT) for secure data transmission and storage.

7.	Application Layer (Layer 7): 

Provides network services directly to end-users and applications, handling high-level protocols like HTTP and FTP.

Security Vulnerabilities:

   - Exploits: Attackers exploit vulnerabilities in software applications to gain unauthorized access or perform malicious actions.
   - Phishing: Social engineering tactics trick users into revealing sensitive information or clicking malicious links.
   - Malware and Exploits: Malicious software or application bugs can compromise security.


Security Measures:

   - Secure Coding Practices: Implement input validation, sanitization, and output encoding to prevent vulnerabilities like SQL injection and XSS.
   - Regular Security Assessments: Conduct penetration testing to identify and fix vulnerabilities.
   - Robust Authentication and Authorization: Use multi-factor authentication (MFA) and role-based access control (RBAC) to protect sensitive data.

<img width="900" alt="image" src="https://github.com/user-attachments/assets/dab4d268-323e-4b6e-8d6a-61f07ac72d08">

_OSI Model as It Relates to Security. Reprinted from SANS Security Essentials GSEC Practical Assignment v1.4b, by Kim Holl, 2003, SANS Institute._

## References

* Bangalore, K. (2023, September 14). Security challenges across network layers (OSI model). Medium. https://medium.com/@kavib/security-challenges-across-network-layers-osi-model-d03d5d187c7
* Froehlich, A., Rosencrance, L., & Gattine, K. (2021, February). OSI. TechTarget. https://www.techtarget.com/searchnetworking/definition/OSI
* InfoSecTrain. (2023, January 25). Common security attacks in the OSI layer model. InfoSecTrain. https://www.infosectrain.com/blog/common-security-attacks-in-the-osi-layer-model/
* Plixer. (n.d.). Network layers explained. Plixer. https://www.plixer.com/blog/network-layers-explained/
* Shaw, K. (2024, July 9). The OSI model explained and how to easily remember its 7 layers. NetworkWorld. https://www.networkworld.com/article/964816/the-osi-model-explained-and-how-to-easily-remember-its-7-layers.html
* [CyberSpecs]. (2024, April 1). Security implementations at different layers of the OSI model. Medium. https://cyberspecs.medium.com/security-implementations-at-different-layers-of-the-osi-model-426df664a766
* Holl, K. (2003). OSI defense in depth to increase application security [Figure 2]. In SANS Security Essentials GSEC Practical Assignment v1.4b. SANS Institute. https://www.giac.org/paper/gsec/2868/osi-defense-in-depth-increase-application-security/104841 








