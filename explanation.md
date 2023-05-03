Choice of the base image on which to build each container.
    - I choose Alpine because it is lightweight and has a small footprint. This means that the image is faster to download, execute and has a smaller attack surface.
Dockerfile directives used in the creation and running of each container.
    - First step i created a dockerignore file to indicate which files not to copy.
    - Second step i create a Docker file in both client and backed and indicate the node version to run, created a folder to copy the files in the home directory and npm start to run the code
Docker-compose Networking (Application port allocation and a bridge network implementation) where necessary.
    - I indicated port 5000 to run the backend and port 3000 to run the frontend.
Docker-compose volume definition and usage (where necessary).
    - I used to docker compose to build both images at a go and indicate the mongo db connection url.
Git workflow used to achieve the task.

Successful running of the applications and if not, debugging measures applied.
    - On cloning the project run "docker-compose up" if the project does not run check the node version installed.
Good practices such as Docker image tag naming standards for ease of identification of images and containers. 
    - I used the semantic tagging that is 1.0.0 since it is my first image.