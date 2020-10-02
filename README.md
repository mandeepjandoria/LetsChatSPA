# LetsChatSPA

# Description
I have created this SPA using Angular 9 (for creating frontend) and Stream-Chat (for chat functionality).
I'm using my stream chat credentials (key and secret) in the .env file in the root folder which can be updated after creating your own stream-chat account.

# Build instructions (Please note point 4 and 5 are optional since you can use my credentials)
1. Clone this repository.
2. Change your directory to this repo.
3. Run `yarn` to install the dependencies
4. Create a stream-chat account and then create an app there.
5. Update the.env file with new key and secret details from your own account.
6. Run 'node server.js' from the project root to start the Node server on port 5500.
7. Run 'ng serve' from the project root to start the Angular app server.
8. View the app by using http://localhost:4200 in your browser.

# Docker file for ease of deployment
I have created the below docker repository which is connected to my github repository:
https://hub.docker.com/repository/docker/deepjandoria/letschatspa_docker

Also, I can install Watchtower on my server which will pull the running docker images and checks for updates. If there are any updates, it will shut down the original container and create a container from the new image with the same settings.

So, now if I push a commit to my GitHub repository, Docker hub will automatically build a Docker image and this image gets pulled by WatchTower and it will run with all original options. In this way, I can automatically deploy my pushed commit (on github) to the server.
