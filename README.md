## reacttypescript
# React boilerplate with typescript including docker configurations. 


 This repo is boilerplate for react typesript.Shared for people who wants to start up new react project easily. 
 react created via cra toolchain with enhanced typescript support. if you want to customize configuration you must first eject cra toolchain that uses react-scripts     for builder. After that read "customize-cra" or other tools on the web. 

 İf you want to run on docker container, you can modify dockerfile.prod, dockerfile.dev and corresponding docker-compose.yml files respectively. 
 it is easy. 

Before production level, do not forget running "npm run build" command on your terminal or ide. 
Test stage skipped,but added related configuration files as well. 

this boilerplate is good choice for medium level applications. 
```markdown
docker : 
development: 
docker-compose -f docker-compose.dev.yml up -d 
docker-compose -f docker-compose.dev.yml up -d --build # for rebuild images and container respectively 
docker-compose -f --rm docker-compose.dev.yml up -d --build # for rebuild images and container respectively and when you shutdown docker it will remove image and container too. 

use same approach for production , before prpduction run "npm run build" 

NOTE: you can use .env file for docker or react app.
