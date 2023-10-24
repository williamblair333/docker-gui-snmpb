# Docker Gui For snmpb

## Features

- Streamlined deployment of SNMP browser with a GUI inside a Docker container.
- Running on Debian Buster Slim i386 with it's dependencies (dpkg -I <package_name>.deb to see them).

- Use this with [Dogma](https://github.com/williamblair333/dogma) for convenience

## Prerequisites

- Docker
- Docker Compose
- X11 Server for GUI

## Directory Structure

docker-gui-gpt4all/  
├── Dockerfile: Defines the Docker container including the necessary dependencies.  
├── docker-compose.yml: Docker Compose configuration file.  
├── snmpb_0.8_i386.deb:  The snmpb package.  
└── logs/: It's supposed to store logs here.  
└── root/: Allows for storing all changes to the running app and will persist on container destruction  
└── tmp/: It might be useful to keep.  

## Getting Started

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/docker-gui-snmpb.git
    cd docker-gui-snmpbrowser
    ```

2. **Build and start the Docker container**:
    ```bash
    docker-compose up --build
    ```

## Notes, Security

- Make sure to handle X11 permissions carefully when granting and revoking access.

## Notes, General

- For better performance, configure your GPU settings appropriately.

## TODO

- Need to test if we need more volumes when adding mibs.  If so, where?  Run docker diff <container_id> to find out!
