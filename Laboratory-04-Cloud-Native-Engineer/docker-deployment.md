# Docker Deployment Log

## Container Lifecycle Commands

| Command | Explanation |
|---|---|
| `docker ps` | Lists all currently running containers along with their ID, image, status, and ports. |
| `docker stop my-nginx` | Sends a stop signal to gracefully shut down the running container. |
| `docker ps -a` | Lists all containers, including stopped ones, confirming the container's status changed to "Exited." |
| `docker rm my-nginx` | Permanently deletes the stopped container and its writable layer. |

## Evidence
See `screenshots/container-lifecycle.png` for terminal output of the full sequence.
