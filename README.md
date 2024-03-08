<h2>Initiate, Capture, and Analyze Telnet Sessions</h2>

<h3>Objectives</h3>
- Establish Telnet connection using provided credentials.
<br />
- Capture Telnet traffic; analyze TCP behavior.
<br />
- Investigate Telnet TCP flags' significance.
<br />
- Assess Telnet security risks; discuss encryption.

<h3>Step 1: Account Creation and Telnet Connection</h3>
In this project, I'll delve into Telnet, contrasting it with its more secure counterpart, SSH. To demonstrate Telnet's functionality, I'll connect to a remote device, tty.sdf.org. To initiate the process, I'll create an account on the website, which will then provide login credentials via email.
<br />
<br />
<img src="https://github.com/Yagoobz/InitiateCaptureAnalyzeTelnetSessions/assets/145611184/fbbada74-43ca-48bb-83cf-1472e0f9687d" height="30%" width="70%" alt="Disk Sanitization Steps"/>

<h3>Step 2: Use Windows PowerShell to Telnet</h3>
Returning to Wireshark, I'll begin capturing traffic on port 23. To generate the traffic, I'll utilize Windows Powershell to telnet to the server. After inputting the username and password received via email, connection is established.
<br />
<br />
<img src="https://github.com/Yagoobz/InitiateCaptureAnalyzeTelnetSessions/assets/145611184/62917b81-8eca-4b0f-b63c-a106de3cb4d7" height="30%" width="70%" alt="Disk Sanitization Steps"/>

<h3>Step 3: Examine Telnet Packet in Wireshark</h3>
I'm examining how TCP sends its traffic in almost real-time. First, I open the initial Telnet packet and delve into the Transmission Control Protocol (TCP). Then, I expand the flags section. I observe that the push flag is set to 1, indicating that whenever a character is received from Telnet, TCP promptly sends it. TCP aggregates the data into a single Protocol Data Unit (PDU) for efficient transmission.
<br />
<br />
<img src="https://github.com/Yagoobz/InitiateCaptureAnalyzeTelnetSessions/assets/145611184/bcbd6a3e-5bea-4f93-840c-24f7dd920e00" height="30%" width="70%" alt="Disk Sanitization Steps"/>

<h3>Step 4: Follow TCP Stream for Telnet</h3>
For further analysis, I right-click on the initial Telnet packet and select "follow TCP Stream." This action reveals the entire Telnet session, indicating that the communication is not encrypted and therefore lacks security measures. Using Telnet for communication with remote devices is insecure and not recommended.
<br />
<br />
<img src="https://github.com/Yagoobz/InitiateCaptureAnalyzeTelnetSessions/assets/145611184/e34aa4e5-d3b5-42ef-bfa5-d70b235a9be3" height="30%" width="70%" alt="Disk Sanitization Steps"/>
