
Docker Compose:

- YAML file consisting of all the details regarding various services, networks, and volumes that are needed for setting up the Docker-based application.
- So, docker-compose is used for creating multiple containers, host them and establish communication between them.
- For the purpose of communication amongst the containers, ports are exposed by each and every container.

Docker Namespace:
- A namespace is basically a Linux feature that ensures OS resources partition in a mutually exclusive manner.
- This forms the core concept behind containerization as namespaces introduce a layer of isolation amongst the containers. In docker, the namespaces ensure that the containers are portable and they don't affect the underlying host. Examples for namespace types that are currently being supported by Docker – PID, Mount, User, Network, IPC.

Docker Commands:
- Docker ps -a:
	- Get status of all the containers
- 