# Developers Social Network

## Table of Contents

- [Packages Production](#packages-production)
- [Packages Development](#packages-development)
- [Build application locally](#build-application-locally)

## Packages Production

- **guzzlehttp/psr7**  
`composer require guzzlehttp/psr7`
- **http-interop/response-sender**  
 `composer require http-interop/response-sender`

## Packages Development

- **codeception**  
`composer require codeception/codeception" --dev`
- **symfony/var-dumper**  
`composer require --dev symfony/var-dumper`
- **suqizlabs/php_codesniffer**  
`composer require --dev squizlabs/php_codesniffer`

## Build Application locally

On your local machine, clone this repo:

```bash
~$ git clone git@github.com:Havet-Vincent/DevelopersSocialNetwork.git
~$ cd DevelopersSocialNetwork
```

Copy file **.env.dist** to **.env** in CLI

```bash
~$ cp .env.dist .env
```

Modify **DB_PWD=xxxx** for password MySql (`the default user is root`)

Then build and run this project

```bash
~$ cd docker
~$ docker-compose up -d --build 
```

Once the container is build and running, visit [http://localhost:8080](http://localhost:8080) in your web browser to view the project.

To stop the staging container, use the `docker-compose down` command:

```bash
~$ docker-compose down
```
