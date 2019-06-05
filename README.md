### Docker compose 
- Apache 2
- PHP 7.2.10
- phpMyAdmin
- MySQL
- MailDev

#### Configuration
Php project location in `source` folder.
Web document root `source/public` can be changed in `.docker/config/vhosts/source.conf` file, by `docrootweb` parameter

#### Initialization
> docker-compose build

At this moment, Docker will execute all configurations that we set up. When it’s done, you can launch your containers !
> docker-compose up -d

#### Usage
Connect to mysql container via bash

> docker exec -it amp_mysql bash

#### Examples connection to docker containers
DB connection: `mysql://amp:amp@mysql:3306/amp`

SMTP connection: `smtp://amp_maildev:25`
 
Those parameters are available in `docker-compose.yml` file.
