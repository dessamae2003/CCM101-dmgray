# Mission 4 Reflection

1. **Boot time/setup comparison**: How does Docker's few-seconds startup compare to installing an OS on a VM (partitioning, config, driver install, etc.)?

2. **Why port mapping matters**: Without `-p 8080:80`, the container's internal port 80 is not reachable from outside. Explain how mapping bridges host and container networking.

3. **What happens on `docker rm`**: Containers are ephemeral by default — explain what happens to any data written inside a container (not in a volume) when it's removed.

4. **DevOps impact**: How does packaging an app with all its dependencies into one image reduce "it works on my machine" problems between developers and ops teams?

5. **Portfolio evolution**: Look back at Labs 1–3 (Welcome to the Cloud, Blueprint, Multi-Cloud Explorer) and describe how this lab builds on those skills.
