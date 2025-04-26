# BancoNe Project

## Overview

This project consists of multiple services including `sistema-core`, `ibanking`, `app-mobile`, and `portal-web`. Each service has its own Dockerfile and is managed using Docker Compose.

## Directory Structure

```
BancoNe/
│── sistema-core/
│   ├── Dockerfile
│   ├── package.json
│   ├── package-lock.json
│   ├── server.js
│   ├── src/
│   └── config/
│
│── ibanking/
│   ├── Dockerfile
│   ├── requirements.txt
│   ├── app.py
│   ├── src/
│   └── config/
│
│── app-mobile/
│   ├── Dockerfile
│   ├── package.json
│   ├── package-lock.json
│   ├── src/
│   ├── public/
│   └── build/ (se genera tras el build)
│
│── portal-web/
│   ├── Dockerfile
│   ├── index.html
│   ├── styles.css
│   ├── app.js
│   ├── assets/
│   └── static/
│
│── nginx/
│   ├── nginx.conf
│
│── ansible/
│   ├── deploy.yml
│   ├── inventory.ini
│
│── .env
│── docker-compose.yml
│── README.md
```

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Create a `.env` file with the necessary environment variables.
4. Run `docker-compose up --build` to start all services.

## Deployment

Use the provided Ansible playbook to deploy the application to your servers.

```sh
ansible-playbook -i ansible/inventory.ini ansible/deploy.yml
```
