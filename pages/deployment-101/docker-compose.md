---
layout: section
---

# Break Time
### 10 minutes


---
layout: section
---

# Hands-On Activity 1
### Build a Working Stack with Docker Compose

---

# Prerequisites
* Docker Compose
* (for Windows) WSL 2 or later

<br>

---
layout: center
---

# Objective
### Turn `ku-polls` into an installable tech stack with Docker

---

# Outline
Let's plan out how we can do so,

* Make a working `Dockerfile` for `ku-polls`.
    * Browse a suitable image in Docker Hub.
    * Omit the unwanted files with `.dockerignore`.
    * Replicate steps to build our application with `Dockerfile`.
* Create a `docker-compose.yaml` with `ku-polls` and `PostgreSQL`.
    * Write a service for database.
        * We'll use the image, `postgres`.
    * Write a service for our application.
* [et voilà!]{style="background: linear-gradient(to right, #ef5350, #f48fb1, #7e57c2, #2196f3, #26c6da, #43a047, #eeff41, #f9a825, #ff5722); -webkit-background-clip: text; -webkit-text-fill-color: transparent;"}

---

# Resources

* My `first.Dockerfile` for building an app.
* My `second.Dockerfile` for use with `docker compose`.
* My `docker-compose.yaml` file.
* My `.env` for populating the compose file.

The resources are all in [here](https://gist.github.com/GToidZ/f5ca4ce98ce206a3dc77d033ff866942).

---

# Consider container services or externalized services
From the activity, we have tried containerized services.

Containerized services can be easily spun and managed by a container controller like Docker.
Using Docker Compose we can create a tech stack that our application requires.

Every services are in the same place, but in return it becomes resource-extensive, unless you have
your own infrastructure, it is not quite possible to deploy this way.

The benefits:
* ✅ Easily recreates services your application needs.
* ✅ Automatically provisions resources for you.
* ✅ Allows your infrastructure to be portable.

---

# Consider container services or externalized services
From the activity, we have tried containerized services.

While most PaaS do support Docker, Docker Compose was not, due to its nature, spinning up a bunch of containers.
Some developers also don't want to manage other services rather than their application.

The solution is to use cloud services and have the application connect to those services instead.
In exchange for managing in keeping track of more resources.

The benefits:
* ✅ Only need to deploy your application.
* ✅ Potentially more features than building a stack from scratch.
* ✅ More choice on where to host your application.