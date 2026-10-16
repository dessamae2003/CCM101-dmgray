# Laboratory 8: The Cloud Security Engineer

## Mission Overview
In this lab, I acted as a Cloud Security Engineer at CloudNova Technologies. I deployed an Nginx web app in a container, then secured the Ubuntu server using UFW with a Default Deny policy, allowing only SSH (22) and the web app (8080).

## Objectives
- Understand Attack Surface and the Principle of Least Privilege
- Audit active ports on a Linux server
- Configure UFW with a Default Deny policy
- Selectively allow SSH and HTTP traffic
- Document firewall rules in Markdown

## Commands Executed
```bash
docker run -d --name secure-web-app -p 8080:80 nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned
- Running containers with port mapping
- Configuring a host-based firewall (UFW)
- Applying Default Deny and least privilege
- Testing connectivity with curl
- Documenting security configurations

