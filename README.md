\# DevOps Portfolio — Docker \& GitHub Actions



A beginner DevOps project demonstrating website containerization with Docker and automated image builds using GitHub Actions.



\## Project Overview



This project packages a simple HTML portfolio website into a Docker container using NGINX. A GitHub Actions workflow automatically builds the Docker image when changes are pushed to the `main` branch or a pull request targets `main`.



\## Technologies Used



\- HTML5

\- Docker

\- NGINX

\- Git and GitHub

\- GitHub Actions

\- YAML



\## Project Structure



```text

devops-portfolio/

├── index.html

├── Dockerfile

├── README.md

└── .github/

&#x20;   └── workflows/

&#x20;       └── docker-build.yml

```



\## Run the Project Locally



\### 1. Clone the repository



```bash

git clone https://github.com/Raheena-07/devops-portfolio.git

cd devops-portfolio

```



\### 2. Build the Docker image



```bash

docker build -t raheena-devops-portfolio .

```



\### 3. Run the container



```bash

docker run --name raheena-portfolio -p 8081:80 -d raheena-devops-portfolio

```



\### 4. Open the website



Visit \[http://localhost:8081](http://localhost:8081).



\### 5. Stop the container



```bash

docker stop raheena-portfolio

```



To remove the stopped container:



```bash

docker rm raheena-portfolio

```



\## Continuous Integration



The GitHub Actions workflow is located at `.github/workflows/docker-build.yml`.



It automatically:



1\. Checks out the repository.

2\. Sets up Docker Buildx.

3\. Builds the Docker image.

4\. Reports the build result in GitHub Actions.



The workflow builds the image but does not publish it to a container registry.



\## Learning Outcomes



\- Creating a Docker image using a Dockerfile.

\- Running a container with port mapping.

\- Managing source code with Git and GitHub.

\- Automating Docker builds using GitHub Actions.

\- Understanding the fundamentals of continuous integration.



\## Future Improvements



\- Deploy the website to a cloud platform.

\- Publish Docker images to a container registry.

\- Add automated tests and deployment workflows.

\- Add monitoring and logging.



\## Author



Raheena Rahuman



GitHub: https://github.com/Raheena-07



