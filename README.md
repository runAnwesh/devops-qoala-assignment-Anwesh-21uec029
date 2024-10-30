# DevOps Assignment Solution: Debugging and Running a Dockerized Application

This document details the process followed to debug, run, and verify a Dockerized application as part of the DevOps assignment.

## Solution Overview

In this solution, the following tasks were completed:
1. Set up Docker and Docker Compose.
2. Built Docker images and launched containers.
3. Debugged and resolved intentional errors in the code to ensure the application ran correctly.
4. Verified the application through browser access and checked web server logs.
5. Documented the debugging process and resolution steps.

---

## Solution Steps

### 1. Initial Setup
1. **Cloning the Repository**
   - Cloned the GitHub repository containing the `Dockerfiles`, `docker-compose.yml` file, and application code.

2. **Building Docker Images**
   - Built Docker images locally for each service using the provided Dockerfiles.
   - Tagged the images as `local-nginx` and `local-python-app` to be referenced in `docker-compose.yml`.

### 2. Running the Docker Compose File
1. **Starting the Containers**
   - Used the `docker-compose.yml` file to launch the containers. An error occurred initially due to intentional code and configuration issues, which were subsequently identified and corrected.

### 3. Debugging and Testing
1. **Identifying Issues**
   - Errors were detected through log analysis and code inspection. Key issues included:
     - Incorrect configuration in `docker-compose.yml` and `Dockerfiles`.
     - Misnamed directories, typos in port numbers, and incorrect EXPOSE statements.

2. **Resolving Issues**
   - Corrected the errors by:
     - Fixing typos in `Dockerfiles` (e.g., `EXPOSE "eight thousand"` changed to `EXPOSE 8000`).
     - Correcting paths and filenames in `docker-compose.yml` and `nginx.conf`.
     - Adjusting `nginx.conf` settings to properly proxy requests to the Python app.

3. **Verifying Access**
   - Accessed the application at `http://localhost` to confirm it was running correctly.
   - Verified Nginx logs to ensure requests were received and routed to the Python application as expected.

### 4. Final Submission
1. **GitHub Repository**
   - Created a new GitHub repository named `devops-qoala-assignment-anwesh`.
   - Uploaded the updated `Dockerfiles`, `docker-compose.yml`, and configuration files.
   - Granted access to `devops@qoala.id`.

2. **Screenshots**
   - Included screenshots of:
     - The application running in the browser.
     - Nginx access logs showing successful requests.

3. **Report**
   - Documented the debugging steps and solution in a one-page report.
