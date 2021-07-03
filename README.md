# docker-laravel 🐳

![License](https://img.shields.io/github/license/ucan-lab/docker-laravel?color=f05340)
![Stars](https://img.shields.io/github/stars/ucan-lab/docker-laravel?color=f05340)
![Issues](https://img.shields.io/github/issues/ucan-lab/docker-laravel?color=f05340)
![Forks](https://img.shields.io/github/forks/ucan-lab/docker-laravel?color=f05340)

## Introduction

Build a simple laravel development environment with docker-compose.

## Usage

```bash
$ git clone https://github.com/AkiraSuzukiJP/docker-laravel.git

$ make create-project # Install the latest Laravel project
$ make install-recommend-packages # Optional
$ make init
$ make npm-install
$ make npm-dev

```

http://localhost

## Tips

- Read this [Makefile](https://github.com/AkiraSuzukiJP/docker-laravel/blob/main/Makefile).
- Read this [Wiki](https://github.com/AkiraSuzukiJP/docker-laravel/wiki).

## Container structures

```bash
├── app
├── web
└── db
```

### app container

- Base image
  - [php](https://hub.docker.com/_/php):8.0-fpm-buster
  - [composer](https://hub.docker.com/_/composer):2.0

### web container

- Base image
  - [nginx](https://hub.docker.com/_/nginx):1.20-alpine
  - [node](https://hub.docker.com/_/node):16-alpine

### db container

- Base image
  - [mysql/mysql-server](https://hub.docker.com/r/mysql/mysql-server):8.0



ブラウザにて http://127.0.0.1へアクセス
