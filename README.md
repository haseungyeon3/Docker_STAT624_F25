# SQL+Python+Rstudio Docker Environment
**Description**: Dockerfiles and docker compose for SQL and Python environment for   STAT 624

## Quick start guide
1. Download zipped folder containing all files in this repository.
2. Unzip folder and store in local directory of your choosing.
3. In a terminal window, navigate to the local directory containing `docker-compose.yml`.
4. Run the command `docker compose up`.  The Docker images will be downloaded to your system and containers will be created accordingly.
5. Open a web browser window and type `localhost:5050` to open pgAdmin4 GUI to interact with the database.
6. In a different web browser tab, copy and paste the custom URL provided in the terminal window to access the Jupyter notebook environment to interact with the database.  

## Creating Images from Dockerfile
1. Open your terminal in the directory containing the Dockerfile.
2. Build the image using: `docker build temp . `
3. Tag the image for Docker Hub:`docker tag temp:latest {yourDockerHubRepo:tagname}`
4. Push the image to Docker Hub:`docker push {yourDockerHubRepo:tagname}`
5. If you want to use your custom image, update the docker-compose.yml file by replacing the image name with {yourDockerHubRepo:tagname}
