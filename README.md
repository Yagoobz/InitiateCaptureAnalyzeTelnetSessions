<h2>Exercise 4: Initiate, Capture, and Analyze Telnet Sessions</h2>

<h3>Objectives</h3>
- ...
<br />
- ...
<br />
- ...
<br />
- ...

<h3>Step 1: Account Creation and Telnet Connection</h3>
In this project, I'll delve into Telnet, contrasting it with its more secure counterpart, SSH. To demonstrate Telnet's functionality, I'll connect to a remote device, tty.sdf.org. To initiate the process, I'll create an account on the website, which will then provide login credentials via email.
<br />
<img src="https://github.com/Yagoobz/InitiateCaptureAnalyzeTelnetSessions/assets/145611184/fbbada74-43ca-48bb-83cf-1472e0f9687d" height="30%" width="70%" alt="Disk Sanitization Steps"/>

<h3>Step 2: Use Windows PowerShell to Telnet</h3>
Returning to Wireshark, I'll begin capturing traffic on port 23. To generate the traffic, I'll utilize Windows Powershell to telnet to the server. After inputting the username and password received via email, connection is established.
<br />
<img src="https://github.com/Yagoobz/InitiateCaptureAnalyzeTelnetSessions/assets/145611184/62917b81-8eca-4b0f-b63c-a106de3cb4d7" height="30%" width="70%" alt="Disk Sanitization Steps"/>

<h3>Step 3: Examine Telnet Packet in Wireshark</h3>
I'm examining how TCP sends its traffic in almost real-time. First, I open the initial Telnet packet and delve into the Transmission Control Protocol (TCP). Then, I expand the flags section. I observe that the push flag is set to 1, indicating that whenever a character is received from Telnet, TCP promptly sends it. TCP aggregates the data into a single Protocol Data Unit (PDU) for efficient transmission.
<br />
<img src="https://github.com/Yagoobz/InitiateCaptureAnalyzeTelnetSessions/assets/145611184/62917b81-8eca-4b0f-b63c-a106de3cb4d7" height="30%" width="70%" alt="Disk Sanitization Steps"/>

