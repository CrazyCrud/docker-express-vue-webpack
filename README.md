# Dockerized Vue, Nodejs Express and Postgres Template

##Develop
Run `docker-compose up` or `docker-compose up -d` to free the terminal.

To install NPM packages for the frontend development process execute the following:
`docker-compose exec web npm i <package-name>`

You can check the *Node* server with `curl -i localhost:8083/` which should return "Hello!"

You can connect to the database via *PG-Admin* by entering the connection details from the ".env" file and you can also
 edit
 the
 "init.sql" file in the "postgres-init
" folder.

## Errors  
Maybe you get the following error:
`Error: Missing binding /usr/src/web/node_modules/node-sass/vendor/linux_musl-x64-64/binding.node`  
While the containers are running execute the following:
`docker-compose exec web npm rebuild node-sass`