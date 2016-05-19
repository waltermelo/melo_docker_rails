# melo_docker_rails
A docker-compose.yml file with a group of containers with a ready to use Rails development environment
this file was developed to be used in a similar way just like a vagrant box

Paste the file in a folder and type:
 docker-compose run --rm --service-ports rails
 
 this will initialize a ready to use rails environment .. just do what you want there ... for example
 rails new app ... and the files will be created in the host machine
 
 
 --service-ports is typed to expose the ports , this way you can acess localhost:3000
 if you want to open a second terminal just don't type it
 docker-compose run --rm rails
 
 
 some features: 
 
 * you can type bundle install and it will save your gems in a separated container that way you cannot need to install them again
 * MYSQL is ready to use .. the default password is 23788
 * files created are not "protected" more .. this way you can edit/delete it anytime you want without needing to type sudo, su everytime
