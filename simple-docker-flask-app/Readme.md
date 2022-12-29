## Simple app deployement using docker on AWS

### Dockerfile
  *John and Melwin are friends who had cooking as their passion. 
  At one point of time John went to London and Melwin stayed at America. 
  John tried a new recipe which tasted deliciously and wanted Melwin to feel the same taste, 
  He can't send the dish to Londo tho.. So he wrote down a recipe list and procedure and
  send the recipe file to Melwin to try.*
  
  Dockerfile is just like the recipelist. It is the blueprint which has the details on what will the image contain and do.
  
### What are we trying here ?
#### Dockerfile : 
   This dockerfile will execute the flask app in container and base image python.3.8. Installs dependencies from requirement.txt. 
   Port exposed is 5000 i.e., port 5000 will be exposed from container.
#### Dockerrun.aws.json
   This file contains the details for deploying our application on AWS server.
 ### Commands for deploying same app
    cd simple-docker-flask-app
    docker build -t <username>/<app name> .
    docker run -p 8888:5000 <username>/<app name>
    flask app will be running at http://localhost:5000/ 
 
        
