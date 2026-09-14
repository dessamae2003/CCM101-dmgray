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
- How to verify Docker is installed and check the status of the Docker environment using `docker --version` and `docker info`.
- How to pull a container image from Docker Hub using `docker pull`.
- How to run a container in detached (background) mode and map a host port to a container port using `docker run -d -p`.
- How to test that a containerized service is reachable using `curl` against the mapped host port.
- How to manage the full lifecycle of a container: listing running containers (`docker ps`), stopping a container (`docker stop`), verifying it has stopped (`docker ps -a`), and removing it completely (`docker rm`).
- How to troubleshoot common container issues, such as a service not being ready yet when tested, or confirming whether a command already executed successfully based on error messages from later commands.
- A clearer understanding of how containers differ from VMs in practice — seeing firsthand how fast an Nginx web server can be deployed and torn down compared to setting up a full virtual machine.

## Challenges Encountered
- After running `docker run` to start the Nginx container, my first `curl http://localhost:8080` attempt failed with a "Connection reset by peer" error. This happened because I ran the pull, run, and curl commands too quickly in succession, before the Nginx service inside the container had fully started. Running `docker ps` confirmed the container was actually up, and re-running `curl` afterward worked correctly.
- When practicing the container lifecycle commands, I initially pasted multiple commands at once, which made it unclear from the terminal output whether `docker rm my-nginx` had actually executed. When I tried to run the lifecycle commands again, I got a "No such container: my-nginx" error, which showed the container had already been removed successfully the first time. I resolved this by redeploying a fresh container and running each lifecycle command (`docker ps`, `docker stop`, `docker ps -a`, `docker rm`) one at a time, confirming each result before moving to the next step.
