# Docker Gui For snmpb

## Features

- Streamlined deployment of SNMP browser with a GUI inside a Docker container.
- Designed to work with Debian-based images satisfying specific dependencies.

- Use this with [Dogma](https://github.com/williamblair333/dogma) for convenience

## Prerequisites

- Docker
- Docker Compose
- X11 Server for GUI

## Directory Structure

docker-gui-gpt4all/  
├── Dockerfile: Defines the Docker container including the necessary dependencies.  
├── docker-compose.yml: Docker Compose configuration file.  
├── gpt4all-installer-linux.run: GPT-4 All installer for Linux.  
└── docs/: LocalDocs for training go here  
└── models/: Model files , set this in the GUI  

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

