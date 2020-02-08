# Apache Guacamole (Docker-Compose edition)

## To enjoy this repo:
* Confirm **Docker** is installed on your system
* **Git clone** this repo.
* Run **docker-compose** and enjoy!

## Instructions & Tips:
### Setting up RDP connection
* In-order to create an RDP connection, make sure to set Security mode to "TLS encryption" and check the "Ignore server certificate"
* In-order to allow RDP sessions to to the Windows login screen, check the "Disable authentication" option.

## Optional:
* Change the default **Root account** password in the MySQL container (./docker-compose.yml)
* Change the **Guacamole account** password in the MySQL container (./guacamole\_db_initdb/02-users.sql)
* Change the contianers **logging** driver to Gelf & direct the logs into ELK

## Release notes:
### Version 0.2 (will be pushed in the near future):
#### Completed:
* Created "/root/.config/freerdp/known_hosts" as it was missing
* Using .env file to set all Docker-Compose variables
* Windows 10 RDP instructions
#### In development:
* Change Guacamole FQDN to not require /Guacamole in the end of its URL
* Confirm changes are saved to the containers!
* Search if possible to configure default configurations for new future connections to be set
### Version: 0.1

### All credits goes to Apache [Ref](https://guacamole.apache.org/doc/gug/guacamole-docker.html)
