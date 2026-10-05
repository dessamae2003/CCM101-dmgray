# Laboratory Activity 7: Mission 7 - The Cloud Operations Engineer

## Mission Overview
Transitioned into a Site Reliability Engineering (SRE) role to establish host baselines, deploy an Nginx web server container, generate simulated web traffic, and analyze system logs and container metrics.

## Objectives
* Establish a hardware and resource baseline for the host server using native Linux CLI tools.
* Deploy containerized web applications and simulate HTTP traffic patterns.
* Extract and interpret application access logs to track error codes.
* Monitor real-time container CPU, memory, and network performance using Docker stats.
* Document observability reports and system health metrics clearly using Markdown.

## Monitoring Commands Executed
* `free -h`
* `df -h`
* `top`
* `docker run -d -p 8080:80 --name client-website nginx`
* `curl http://localhost:8080`
* `curl http://localhost:8080/hidden-admin-page`
* `docker logs client-website`
* `docker stats`
## Skills Learned
* Linux resource profiling and baseline health checking.
* Container lifecycle management and traffic simulation.
* Log analysis and HTTP status code troubleshooting.
* Real-time container metrics observation and infrastructure documentation.
