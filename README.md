# Hello World

A simple example project for [Ansible Container](https://github.com/ansible/ansible-container).

## Prerequisites

- [Ansible Container 0.9.2+](http://docs.ansible.com/ansible-container/installation.html)
- Access to a Docker daemon

## Run it!

The following script will download this project from Galaxy, build the container, and run it locally, exposing the flask server on host port 4000:

```
#!/bin/bash
# Create a new directory, and set it as your working dir
mkdir hello-world
cd hello-world 

# Download the project
ansible-container init ansible.hello-world

# Build the container
ansible-container build 

# Run hello world
ansible-container run

# Open a browser and load http://localhost:4000
open http://localhost:4000
```

