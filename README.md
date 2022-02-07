# Red-vs-Blue-Team-Project
Cybersecurity Exercise:  Defense and Offensive sides
The exercise began with recon of the machines, determining 192.168.1.90 was the attacking machine and 192.168.1.105 was the target machine.  Open Ports were determined as 22 and 80; concentration on Port 80. Using Crack-the-hash to obtain usernames and passwords the payload was set to php/meterpreter/reverse_tcp allowing multi/handler to open meterpreter which allows access to the machine's shell.  Kibana was used to visualize the peak in network traffic.

Brute force is seen in HTTP 200, 301 and 400; 30 successful attacks returned the status code of move permanently.  The attacker was successful in finding the web based distributed authoring and versioning (WebDav), a set of extensions to the HTTP protocol allowing users to edit and manage files on remote web servers.

Risk mitigation utilizes security policies and procedures to reduce the impact of a threat; typically, prevention, prevention, detection and remediation. In this exercise the mitigation was separated into the following: Prevention of Brute Force Attacks, the WebDav connection and Reverse Shell uploads.

This report concludes with a suggestion to limit the number of shared folders and restrict the WebDav folder to read only, preventing uploads into the folder.  Blocking all IP’s is not realistic however, tracing activity of the IP’s, keeping record and forwarding suspicious IP addresses to an internal repository will aid in keeping a watchful eye for those which require blocking.
