# Mission 8 Reflection

**1. How does a host-based firewall protect a server even if the physical network perimeter is breached?**
A host-based firewall filters traffic on the server itself, so it keeps working even if an attacker gets past the network edge. If someone is already inside the network, UFW still drops any connection to ports that were not explicitly allowed. This is defense in depth: no single layer is trusted to stop every threat.

**2. Why is managing open network ports critical to reducing a server's attack surface?**
Every open port represents a running service that someone can connect to, and every service may have vulnerabilities, weak credentials, or misconfigurations. Closing unnecessary ports shrinks the attack surface, giving attackers fewer entry points and giving administrators less to monitor and patch.

**3. In a real enterprise environment, why is it dangerous to leave a database port (like 3306 for MySQL) open to the public internet?**
Automated scanners find exposed database ports within minutes and launch brute-force or exploit attempts. A successful breach could expose or destroy customer records, leading to financial loss, legal consequences, and damaged reputation. Databases should only be reachable from the application server or a private network.

**4. How did completing this mission change your perspective on how easily a server can be compromised?**
This mission showed me how easily a server can be left exposed. Before enabling UFW, every port was reachable by anyone, and it only took a few commands to change that. I realized that many security failures come from forgotten configuration, not from sophisticated hacking.

**5. How does your GitHub portfolio currently look with eight completed missions?**
My portfolio now contains eight missions covering cloud basics, infrastructure, containers, data, deployment, operations, and security. Each folder has documentation, screenshots, and a reflection, showing my progress from understanding concepts to doing hands-on engineering work.
