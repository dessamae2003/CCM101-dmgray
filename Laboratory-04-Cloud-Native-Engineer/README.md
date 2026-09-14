# Laboratory 04: Cloud-Native Engineer

## Mission Overview
This lab covers the shift from traditional Virtual Machines to lightweight, portable Containers. Using a KillerCoda Docker environment, I deployed a live Nginx web server and documented the full container lifecycle.

## Objectives
- Differentiate between traditional Virtual Machines (VMs) and Containers
- Access a Docker-enabled cloud environment using KillerCoda
- Execute fundamental Docker CLI commands
- Pull, run, manage, and terminate a containerized application (Nginx)
- Create professional technical documentation using Markdown
- Continue developing a well-organized GitHub Cloud Computing Portfolio

## Docker Commands Executed

\`\`\`bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx
\`\`\`

## Skills Learned
- [fill in with your own words, e.g. Docker CLI fundamentals, image vs. container concept, detached mode, port mapping, container lifecycle management]

## Challenges Encountered
- [fill in with your own words, e.g. any syntax issues, port conflicts, or confusion between `docker ps` and `docker ps -a`]
