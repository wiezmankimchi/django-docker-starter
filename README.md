Starter Django on Docker

# to start the docker
> docker-compose up

# to connect to the docker
get the docker container name/ID from the  list of containers
> docker ps

run the following to connect to the docker container
> docker exec -it <container ID> /bin/bash

# deploy db model changes
within the container
> python manage.py makemigrations
> python manage.py migrate

create super user
> python manage.py createsuperuser

User: root
password: welcome2019



# to shut down all containers
> docker-compose down
