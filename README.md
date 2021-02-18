# Docker Symfony 5 with Nginx - PHP - MySQL

## Install  

Place the folder at the root of your project and rename it "docker".<br>
Copy .env.local.example and remane it .env.local at the root of your project

## Versions

This docker is running : 
- PHP 8.0.1 (PHP 8.1 ASAP)
- MySQL 8.0.23
- Nginx 1.19.6
- NodeJS 14.15.5
- NPM 6.14.11

## Commands

- Build

```bash
docker-compose -f ./docker/docker-compose.yml build
```

- Build & Up (No daemon)

```bash
docker-compose -f ./docker/docker-compose.yml up --build
```

- Up (No daemon)

```bash
docker-compose -f ./docker/docker-compose.yml up
```

- Up (With daemon)

```bash
docker-compose -f ./docker/docker-compose.yml up -d
```

- Access to PHP container
```bash
docker exec -ti app bash
```

- Stop

```bash
docker-compose -f ./docker/docker-compose.yml stop
```

- Down

```bash
docker-compose -f ./docker/docker-compose.yml down
```

## Troubleshooting

If something is missing for your project or if you are struggling with this docker don't hesite to create an issue
