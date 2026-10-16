# Security Audit Report

## 1. The Principle of Least Privilege (PoLP)
The Principle of Least Privilege means giving every user, account, or application only the minimum permissions it needs to do its job, and nothing more. It is important for cloud user accounts because if one account is stolen or misused, the damage is limited to what that account could access. Without it, a single compromised account could give an attacker control of the whole environment.

## 2. Attack Surface
The attack surface of a virtual machine is the total of all the points where an attacker could try to get in. This includes open network ports, running services, installed software, and user accounts. The more services and ports a VM exposes, the larger its attack surface and the more chances an attacker has to find a weakness.

## 3. Default Deny Policy
A Default Deny policy blocks all incoming traffic unless it is explicitly allowed. It is safer than blocking hackers one by one because it is impossible to know every malicious IP address or attack method in advance. By contrast, the list of services a server actually needs is short and known, so allowing only those leaves everything else protected automatically.
