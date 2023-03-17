# Commands-repository

This is a list of all the **useful** commands you may need while working.

You will find commands for the following applications:
+ [GNU Bash](https://www.gnu.org/software/bash/)
+ [Ubuntu](https://ubuntu.com/)
+ [Git](https://github.com/)
+ [Docker](https://www.docker.com/)
+ [Docker-compose](https://docs.docker.com/compose/)
+ [Terraform](https://www.terraform.io/)

### BASH
```bash
# Show a list of files and folders
ls

# Change directory
cd <directory-path>

# Print working directory command in Linux
pwd

# Print any text that follows the command
echo

# Delete files or directories
rm

# Create blank/empty files
touch

# Access manual pages for all Linux commands
man

# Get the active username
whoami

# Search for a string within an output
grep

# Display disk filesystem information
df

# Command to change file permissions
chmod

# Package managers depending on the distro
apt, pacman, yum, rpm

# Generate ssh key
ssh-keygen -t rsa -b 4096

# Connect to ssh session
ssh <user-name>@<ip-distant-machine>

# Create a user with active bash and password setup
useradd --create-home --shell /bin/bash --password <yourpassword> <user-name>

# Create a directory
mkdir <directory-name>
```


### GIT

```bash
# Initialize a local Git repository
git init

# Configure the author name
git config --global user.name "<username>"

# Configure the author email address
git config --global user.email <email-address>

# Link a remote repository to local
git remote add origin git@github.com:URL/repository.git

# Create a local copy of a remote repository
git clone git@github.com/<username>/<repository-name>.git

# Check status
git status

# Add file to staging area
git add <file-name>

# Commit a change
git commit

# List branches
git branches

# Create a new branch
git branch <branch-name>

# Switch branch
git checkout <branch-name>

# Create a branch and make it active
git checkout -b <branch-name>

# Merge a branch
git merge <branch-name>

# Delete a branch
git branch -d

# Push changes to remote repository
git push

# Push a branch to your remote repository
git push origin <branch-name>
```

### DOCKER

```bash
# Check docker version
docker version

# List all docker images
docker images

# Create a docker image
docker build -t <image-name>

# Run a docker image
docker run <image-name>

# Show running containers
docker ps

# Launch a bash session inside container
docker exec -ti <image-name> /bin/bash

# Stop container
docker stop <image-name-or-id>

# Start a stopped container
docker start <container-name-or-id>

# Fetch the logs of any container
docker logs <container-name-or-id>

# Reveal low-level information about both containers and images
docker inspect <container-or-image-name-id>
# Remove container
docker rm <image-name-or-id>
```

### DOCKER-COMPOSE
```bash
# Create and Start all Containers, Volumes, Images, and Networks in a Docker Compose File
docker-compose up

# Stop and Remove all Containers, Volumes, Images, and Networks in a Docker Compose File
docker-compose down

# Start Services in a Docker Compose File
docker-compose start

# Start Services in a Docker Compose File in background
docker-compose up -d

# Start Services in a Docker Compose File in interactive mode
docker-compose up -it

# Stop Services in a Docker Compose File
docker-compose stop

# Remove Stopped Containers in a Docker Compose File
docker-compose rm

# List Containers Deployed from a Docker Compose File
docker-compose ps

# List images from a Docker Compose File
docker-compose images
```

### TERRAFORM
```bash
# Prepare your working directory for other commands
terraform init

# Get a list of available commands for execution with descriptions
terraform -help

# Validate the configuration files in your directory
terraform validate

# Check whether the configuration is valid
terraform validate

# Show changes required by the current configuration
terraform plan

# Create or update infrastructure
terraform apply

# Destroy previously-created infrastructure
terraform destroy
```

### KUBERNETES
```bash
# Generate a list of all namespaces
kubectl get namespaces

# Show a list of all pods
kubectl get pods

# Show a detailed list of all pods, containing information such as node name
kubectl get pods -o wide

# Show a list of all pods running on a particular node server
kubectl get pods --field-selector=spec.nodeName=<server-name>

# Create a new namespace
kubectl create namespace <namespace-name>

# Create a new service with the definition contained in a [service-name].yaml file
kubectl apply -f <file-name.yaml>
```


