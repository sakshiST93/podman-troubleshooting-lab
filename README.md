# podman-troubleshooting-lab
# Lab: Troubleshooting WordPress Containers

## Objective

Troubleshoot a containerized WordPress application using Podman.

## Components

- sks-backend-ts (MariaDB)
- sks-wp-app-ts (WordPress)
- sks-frontend-ts (NGINX)

## Outcomes

- Create Podman networks
- Create Podman volumes
- Deploy multiple containers
- Configure networking
- Configure port forwarding
- Troubleshoot containers

## Requirements

- Podman installed
- Git installed

## Instructions

1. Create the network:
   podman network create sks-wp-ts

2. Create the volumes:
   podman volume create sks-backend-ts-vol
   podman volume create sks-wp-app-ts-vol

3. Start the containers according to the lab requirements.

## Validation

- All three containers are running.
- All containers are connected to `sks-wp-ts`.
- Volumes are mounted correctly.
- The frontend exposes port **8004**.
- Visit **http://localhost:8004** to verify the application.
