# CTC Remote Internship Web Project - Docker Setup

This project contains a static multi-page website built with HTML, CSS, JavaScript, Bootstrap, and Tailwind CSS. It is containerized using Docker with Nginx to serve the site efficiently.

---

## Project Structure

- `final/` - Contains the HTML files, CSS file, and images.
- `Dockerfile` - Docker configuration to build the container image using Nginx.

---

## Prerequisites

- Docker installed on your system.

Download Docker from [https://www.docker.com/get-started](https://www.docker.com/get-started) if it is not already installed.

---

## Setup Instructions

1. **Clone or download the repository**

```
git clone https://github.com/JabezJoshwin/CTC-Remote-Internship.git
cd CTC-Remote-Internship/final
```

2. **Build the Docker image**

Run this command in the root of your project directory (where the Dockerfile is located):

```
docker build -t ctc-remote-internship .
```


3. **Run the Docker container**

Run the container and map port 80 of the container to your machine's port 80:

```
docker run -p 80:80 ctc-remote-internship
```


4. **Access the website**

Open a web browser and navigate to `http://localhost` (or `http://<your-docker-host-ip>` if running remotely).

---

## Stopping the Container

- To stop the container, press `Ctrl + C` in the terminal running the container.

- Alternatively, list running containers:

```
docker ps
```


Then stop the container by ID:

```
docker stop <container-id>
```


---

## Additional Notes

- Ensure port 80 is free on your host machine before running.
- To use a different port, modify the `docker run` command. For example, to use port 8080:
```
docker run -p 8080:80 ctc-remote-internship
```

Access the site at `http://localhost:8080`.

- This Docker image uses Nginx to serve the static website files efficiently.

---

## Contact

For any issues or questions regarding this project containerization or setup, please contact jabezjoshwin@gmail.com.

---
