
# Déploiement d’une App sur ECS et RDS

![](<Architecture App.png>)

## Useful links:

## Cost estimation: Estimation.pdf

## Features:
- Deployment of a highly available and resilient application at two levels: Presentation & business layer and database layer: WordPress case
- Auto scaling
- Load Balancing
- Data persistence

## Services:

### Network
- **VPC (Virtual Private Cloud)**: Provides an isolated network in the cloud, allowing to define subnets, security rules, and connections to the Internet.
- **SUBNET (Subnet)**: Divides a VPC into smaller segments to organize resources and manage security.
- **INTERNET GATEWAY**: Allows communication between resources in a VPC and the Internet.
- **EIP (Elastic IP)**: Static IP address that can be associated with an instance to make it accessible on the Internet.
- **ALB (Application Load Balancer)**: Distributes inbound traffic across multiple targets (EC2 instances, containers, etc.) and helps manage content-based routing.
- **ACL (Access Control List)**: Defines security rules to control inbound and outbound traffic at the subnet level.
- **NAT (Network Address Translation)**: Allows instances in a private subnet to access the Internet without exposing their IP addresses.
- **ROUTE (Routing Table)**: Defines routing rules to direct traffic between subnets and to the Internet.
- **SECURITY GROUP**: Acts as a virtual firewall to control inbound and outbound traffic for instances.

### Network and DNS
- **ROUTE 53**: DNS service that helps manage domain names and direct traffic to AWS resources.

### Security
- **SECRET MANAGER**: A service that securely stores and manages secrets (such as passwords and API keys).
- **IAM (Identity and Access Management)**: Defines what users and roles can do with AWS resources.
- **Role**: An IAM role is an entity that defines a set of permissions to perform actions on AWS resources. Unlike users, roles are not associated with a specific person or account, but can be assumed by AWS services, users, or applications. Roles are often used to grant temporary permissions.
- **Permission**: Defines what users and roles can do with AWS resources.
- **AWS Certificate Manager (ACM)**: Provisions, manages, and deploys public and private SSL/TLS certificates to secure communications with AWS services and connected internal resources12.

### Storage
- **S3 (Simple Storage Service)**: An object storage service for storing and retrieving data at any time.
- **EFS (Elastic File System)**: A scalable file system that can be mounted across multiple EC2 instances.

### Database
- **RDS (Relational Database Service)**: A managed relational database service for MySQL, PostgreSQL, Oracle, SQL Server, and MariaDB.

### Compute (Containers)
- **ECS (Elastic Container Service)**: A container orchestration service that makes it easy to deploy and manage containerized applications.
- **Fargate**: A serverless compute service that allows you to deploy and manage containers without having to manage the underlying infrastructure. It works with services like Amazon ECS (Elastic Container Service) and Amazon EKS (Elastic Kubernetes Service).
- **Task**: A unit of work in ECS that defines a set of containers to run together.
- **Task Definition**: A template that defines parameters for ECS tasks, including container images, resources, and network configurations.
- **Auto Scaling**: Monitors your applications and automatically adjusts capacity to maintain consistent, predictable performance at the lowest possible cost.

### Resource Monitoring and Management
- **CLOUDWATCH**: A monitoring service that collects and tracks metrics, logs, and events for AWS resources.
- **Container Insight**: A monitoring tool for containers.
- **Logs Groups**: Groups logs together for centralized management and analysis.

  
