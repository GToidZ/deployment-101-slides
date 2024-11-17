---
layout: section
---

# Platform as a Service (PaaS)

---

# What is PaaS?
One of the cloud hosting methods to take note of.

Platform-as-a-Service is a service model made specifically for **cloud computing**. On the platform, users can:
* Provision
* Instatiate
* Manage

...a modular suite of computing modules and services.

---

# Differences from SaaS or IaaS
Even if they looked the same, they really are not.

PaaS targets the means of deploying applications on to the platform based on user needs, these services excel
in creating different environments for different clients. PaaS prepares environment that you can customize freely.

SaaS is **not** the same as above, they offer complete software for end-users, e.g. Google Suite, Slack etc.

IaaS is almost similar to PaaS, the main difference is that they offer more versitility in what kind of resources
build your entire system. This can be a turn-off for new developers since you are responsible for building what your application runs on.

---
layout: image-right
image: ./assets/heroku-logotype-vertical-purple.png
---

# Example: [Heroku](https://www.heroku.com/)
Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud. Heroku offers **tiered** pricing model, and each service consists of different tiers.

### Pros ✅
* Applications integrates seamlessly with version control servers like GitHub.
* The services on platform can always be scaled to meet the demands of traffic.

### Cons ❌
* Idle applications will be put to sleep.
* Its database does not scale indefinitely due to tiered pricing.

---
layout: image-right
image: ./assets/PA-logo-large-icononly.png
---

# Example: [PythonAnywhere](https://www.pythonanywhere.com/)
PythonAnywhere makes it easy to create and run Python programs in the cloud. It has a free tier which is very limited.

### Pros ✅
* Setup your deployment like in your machine, with sufficient tools included.
* You can deploy stateful applications and data will persist.

### Cons ❌
* Supports only Python.
* Your application can only communicate with trusted URLs. (free tier)

---

# More Examples

* [fly.io](https://fly.io/)
* [Google App Engine](https://cloud.google.com/appengine)
* [Railway](https://railway.app/)