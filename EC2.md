# How to set up AWS EC2 instance for Code Elevate

This guide provides step-by-step instructions to set up an AWS EC2 instance with the necessary dependencies to run the Code Elevate system.

In this guide, you will install the following prerequisites:

- Git
- Docker
- Docker Compose
- Node.js
- npm

## Step 1: Launch an EC2 instance

1.1. Open the Amazon EC2 console at https://console.aws.amazon.com/ec2/.

1.2. From the console dashboard, choose Launch Instance.

1.3. The Choose an Amazon Machine Image (AMI) page displays a list of basic configurations, called Amazon Machine Images (AMIs), that serve as templates for your instance. Select an AMI, such as Amazon Linux 2 AMI.

1.4. On the Choose an Instance Type page, you can select the hardware configuration of your instance. Select the t2.micro type, which is selected by default.

1.5. Choose Review and Launch to let the wizard complete the other configuration settings for you.

1.6. On the Review Instance Launch page, under Security Groups, choose Edit security groups.

1.7. Add a rule to allow inbound traffic to your instance. The Engine uses port 2000. You can add a rule to allow inbound traffic to port 2000 from anywhere.

1.8. Connect to your instance. You can connect to your instance using the Amazon EC2 console.

## Step 2: Install the prerequisites

2.1. Update the installed packages and package cache on your instance.

```bash
sudo yum update -y
```

2.2. Install the Git, Docker, Node.js, and npm packages.

```bash
sudo yum install git docker nodejs npm -y
```

2.3. Configure the Docker daemon and start Docker.

```bash
sudo service docker start
sudo chmod 777 /var/run/docker.sock
```

2.4. Install Docker Compose.

```bash
sudo curl -L --fail https://raw.githubusercontent.com/linuxserver/docker-docker-compose/master/run.sh -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

## Step 3: Check the installation

3.1. Verify that Docker and Docker Compose are installed correctly.

```bash
docker --version
docker-compose --version
```

3.2. Verify that Node.js and npm are installed correctly.

```bash
node --version
npm --version
```

---

**Congratulations!** You have successfully set up an AWS EC2 instance with the necessary dependencies to run the Code Elevate system.
