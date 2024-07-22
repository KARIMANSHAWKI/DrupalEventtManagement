
## Intro

This project about event management system using Drupal.


## Installation and usage instructions

 Setup Environment:


I use docker compose to setup environemnt then you need to run these 

```bash
docker-compose up -d --build
```
to access php container

```bash
docker exec -it container_name bash
```

## Install Project Dependencies

1- access php container 

```bash
docker exec -it container_name bash
```

1- Install composer dependencies 

```bash
composer install
```


## Installation of Event Management Module

 From UI:
 
1- Go to Manage → Extend or navigate directly to /admin/modules. <br>
2- Filter existing modules with Events Management.<br>
3- Click install.<br>

 From Cmmand line:
 
 1- Access php container

```bash
docker exec -it php-container bash
```
2- run enable custom module command

```bash
 ./vendor/bin/drush en events_management
```

After Install events management module you can navigate directly to /events 

## Update Event Management Module Config

 Navigate directly to /admin/config/event-api. <br>

