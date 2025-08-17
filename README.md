 # SYN flood attack detection and response using Wireshark

 NOTE: This project is just a lab activity from a Network Security course I took online. The work that I actually did was writing a clear incident report for a security incident in the scenario. In essence, the main goal for the activity was actually for me to write a clear security incident report. Aside from the incident report, the rest of the content below detailing all what I did is fictional and actually gotten from the scenario.

WHAT THIS PROJECT IS ABOUT

This project shows how I investigated a cyberattack on a company’s web server. The company's website suddenly went offline, and I was assigned to find out why.
I used a tool called Wireshark to look at network traffic (data going to and from the web server) and found something unusual—tons of repeated requests trying to connect to the server. These came from a suspicious IP address and overwhelmed the server, making it crash.

WHAT I DID

1. Detected the issue: An alert told me the web server wasn’t responding.
2. Checked the website: I got a "connection timeout" error.
3. Captured network data: I used Wireshark to see what was happening behind the scenes.
4. Spotted the attack: I saw a flood of SYN packets—this is the first step of a connection handshake, but the rest of the steps were missing. This is a SYN Flood Attack (a type of DoS attack).
5. Responded to the attack: Took the server offline temporarily. Blocked the attacker’s IP address in the firewall.
6. Reported the incident to my manager with a summary of what happened, how it worked, and what should be done next.

WHAT YOU'LL FIND IN THIS Repo (Attached files)

- SCENARIO.docx: The fictional scenario explaining what happened.
- How to read a Wireshark TCP_HTTP log.pdf: A beginner-friendly guide that helped me understand the traffic logs.
- Cybersecurity incident report.pdf: A sample report showing how I documented the attack and explained it in simple terms.

WHAT I LEARNED

- How SYN Flood attacks work by abusing the TCP handshake process.
- How to recognize abnormal traffic using Wireshark.
- How to respond quickly to a DoS attack by isolating the server and blocking attackers.
- How to write a clear incident report.

WHO THIS IS FOR

- Beginners learning about cybersecurity attacks.
- Anyone wanting to practice analyzing network traffic.
