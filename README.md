# WordPress on AWS EC2 using Docker

This project deploys WordPress with MySQL on AWS EC2 using Docker Compose.

## Tech Stack
- AWS EC2 (Ubuntu)
- Docker & Docker Compose
- WordPress Latest
- MySQL 8

## Architecture
User -> EC2 (Port 80) -> WordPress Container -> MySQL Container (wpdb)

Both containers are connected through a custom Docker network `wpnet`.

## Deployment Steps
1. Launched an EC2 instance
2. Installed Docker on EC2
3. Created `docker-compose.yml` for WordPress and MySQL
4. Deployed using `docker compose up -d`

## How to Run
```bash
git clone <your-repo-link>
cd wordpress-ec2-docker
docker compose up -d