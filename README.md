# docker-common-servers
common servers that are used in development, like mysql, posgresql, redis and so on. Inspired by the laradock project, http://laradock.io/

# Usage:

Make sure you have docker installed and running properly

In the project directory

- adjust the configuration: `cp .env.example .env`, end edit .env file with your settings
- `docker-compose up -d <list of services to activate>` - check the docker-compose.yml file for the list of services and default ports  
  example:
  
      docker-compose up -d postgres pgadmin
    
  This will start postgres sql server and an admin interface on port 5050. Default user and pass is `default\secret`

The first run will take a while because it needs to download and build the images. Afterwards you will be able to access the
services on their respective ports.
