# Session-3
In this Session we are going to learn how to use PySpark and another Big Data tools.

## Configuration
1. Install dependencies:
```
sudo yum update
sudo amazon-linux-extras install 33
sudo yum install git
sudo yum install -y docker
sudo service docker start
sudo usermod -a -G docker ec2-user
exec $BASH
```

2. Download a Jupyter image with Spark:
```
## Spark and Jupyter image
docker run -v ~/Session-3/work:/home/jovyan/work -d -p 8080:8888 jupyter/pyspark-notebook
 
## Allow preserving Jupyter notebook
sudo chown 1000 ~/Session-3/work
 
## Install tree to see our working directory next
sudo yum install -y tree

# Verify container name
docker ps

# Enter to your container shell
docker exec -it #someHashValue /bin/bash

# Ask for yout Jupyter token access
jupyter server list
```
