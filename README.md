# Git-GitHub-Actions-Docker-hub

This repository demonstrates a complete CI/CD pipeline using **Git**, **GitHub**, **GitHub Actions**, and **Docker Hub**.  
It builds a Docker image with **Nginx** serving a static HTML page that displays: **Welcome "IAM-SIVA-PRASAD"**

The workflow automatically:
- Builds the Docker image from the `Dockerfile`.
- Pushes the image to Docker Hub (`golisivaprasad/siva-web`).
- Uses GitHub Actions for automation.

========================================================================

**Steps:**
1. creste an repo in github.
2. create  an github actions file.
3. create an dockerfile & Index.html file.
4. create an Docker hub account.
5. create an secrets in Github project secrets and variables
6. try to push your code to GitHub its auto matically triger and runn the pipelice and it push the code in to youe desired Docker HUb.

# after created the image you need to test the image.  weather its working or not, by using these commands:

Thi step for download the Docker Image.
**$docker pull golisivaprasad/siva-web:latest**

This command to run Docker Image locally , using this Port Number 8080. !!! 

**$docker run -d -p 8080:80 golisivaprasad/siva-web:latest**

Now chcek the output!. its shouls be look like this if it run Successfully. 

The last command to display the Output

**$ curl http://127.0.0.1:8080**

**OUTPUT**

========================================================================
<!DOCTYPE html>
<html>
<head>
</head>
<body>
    <h1>Welcome "IAM-SIVA-PRASAD"</h1>
</body>
</html>
========================================================================

