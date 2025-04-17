🐳 Docker Overview

What is Docker?
Docker is an application that runs containers on your machine.

It is a centralized, open-source platform designed to build, test, deploy, and run applications efficiently using containerization.

Docker provides all the necessary tools to handle distributed applications in a lightweight and scalable way.

Docker is written in Go programming language.

Docker uses containers that run directly on the host OS (not inside full VMs).

While Docker can be installed on any OS, the Docker Engine runs natively on Linux distributions.

Docker enables OS-level virtualization, also known as containerization.

It was initially released in March 2013 (not 2023) and was developed by Solomon Hykes and Sebastien Pahl.

🖥️ VM vs Container (with Microservices Example)

💡 Virtual Machines (VMs):
VMs are created using hypervisors on a physical server.

Each VM has its own OS and resources (heavyweight).

Example (Roboshop Microservices):

Cart → separate VM

User → separate VM

Catalogue → separate VM

This is resource-heavy and leads to higher overhead.

📦 Containers:
Containers are lightweight and share the host OS kernel.

Multiple containers can run inside a single VM.

Example (Roboshop Microservices):

One VM running:

Cart → container

User → container

Catalogue → container

This improves resource utilization and is much more efficient.

🛠️ Docker Installation on AWS EC2

Step-by-Step Guide:
1. Create an EC2 Instance
Go to AWS Console.
Launch an instance using Amazon Linux 2 or Amazon Linux 2023.
2. Update Your System
$sudo yum update -y
3. Install Docker
For Amazon Linux 2:
$sudo amazon-linux-extras install docker
For Amazon Linux 2023:
$sudo yum install -y docker
4. Start the Docker Service
$sudo service docker start
5. Add Your User to Docker Group
$sudo usermod -a -G docker ec2-user
6. Reconnect SSH
Close your terminal.
Reconnect using SSH to apply new group permissions.
7. Verify Docker Installation
$docker ps

You should see an empty container list output (no errors), confirming Docker is installed and working.