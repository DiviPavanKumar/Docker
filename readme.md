A Comprehensive Guide to Docker: The Modern Containerization Tool

Introduction to Docker
Docker is a powerful, open-source platform designed to simplify the process of building, running, testing, and deploying applications using containerization. It provides an efficient way to develop distributed applications by packaging software into standardized units known as containers.

- Written in: Go Language
- Type: Open-source
- Developed by: Solomon Hykes and Sebastian Pahl
- Initial Release: March 2013

Docker allows applications to be isolated in containers, enabling more efficient resource utilization and consistency across different environments. While Docker can be installed on any operating system, the Docker Engine natively runs on Linux distributions. This container-based virtualization is often referred to as OS-level virtualization.
Virtual Machines vs Containers
Virtual Machines (VMs):
A single physical server can be logically divided into multiple virtual machines using a hypervisor. Each VM includes a full OS and can run applications independently.

Example: Microservices for Roboshop Project using VMs:
- Cart Service -> VM
- User Service -> VM
- Catalogue Service -> VM

Containers:
Unlike VMs, containers share the host OS kernel and isolate application processes. Multiple containers can run inside a single VM, making better use of system resources.

Example: Roboshop Project using Containers:
- One VM hosts multiple containers:
  - Cart -> Container
  - User -> Container
  - Catalogue -> Container

Installing Docker on Amazon Linux (EC2)
- Step 1: Launch an EC2 Instance
Go to AWS Console and create a new EC2 instance.

- Step 2: Update Package Cache
$ sudo yum update -y

- Step 3: Install Docker
- For Amazon Linux 2:
$ sudo amazon-linux-extras install docker

- For Amazon Linux 2023:
- $ sudo yum install -y docker

- Step 4: Start Docker Service
- $ sudo service docker start

- Step 5: Add User to Docker Group
- $ sudo usermod -a -G docker ec2-user

- Step 6: Reconnect to Your Instance
- Log out and log back in to apply group changes.

- Step 7: Verify Docker Installation
- $ docker ps
- Understanding Docker Components
- Image:
- An image is a lightweight, standalone package that includes everything needed to run a piece of software: - code, runtime, libraries, and environment variables.

- Container:
- A container is a runnable instance of an image.

- Docker Hub:
- A cloud-based registry where Docker users can store and share container images.

- Common Docker Commands
- docker images - List all images
- docker pull <image>:<version> - Download image from Docker Hub
- docker create <image> - Create container from image
- docker ps -a - List all containers (including stopped ones)
- docker ps - List running containers
- docker start <container> - Start an existing container
- docker stop <container> - Stop a running container
- docker run <image> - Pull, create, and start a container
- docker rm $(docker ps -a -q) - Remove all containers
- docker rmi $(docker images -q) - Remove all images
- docker rmi <image-id> - Remove specific image
- Port Forwarding in Docker
- Each container, like a server, has its own port range (0-65535). 

- To expose a container's service to the - host machine:

- docker run -p <host-port>:<container-port> <image>

- Foreground Mode:
- docker run -p 8080:80 nginx

- Background Mode:
- docker run -d -p 8080:80 nginx
 
- Useful Docker Commands
- Access container shell:
- docker exec -it <container-id> bash

- Set custom container name:
- docker run -d --name mynginx -p 8080:80 nginx

- View container logs:
- docker logs <container-id>

- Interview Questions on Docker

1. How can you do port forwarding in Docker?
   - Foreground: docker run -p <host-port>:<container-port> <image>
   - Background: docker run -d -p <host-port>:<container-port> <image>

2. How do you access a running container?
   - docker exec -it <container-id> bash

3. How to list all Docker containers including stopped ones?
   - docker ps -a

4. How do you remove all Docker containers?
   - docker rm $(docker ps -a -q)

5. What is the difference between Docker image and container?
   - Image is a static package; container is the running instance of that image.

- Conclusion
- Docker revolutionizes how modern applications are built and deployed. Its lightweight and consistent containerized approach simplifies development workflows and enhances resource efficiency. Whether you're building microservices or deploying production-ready applications, Docker is a must-have tool in every DevOps engineer's toolkit.
