---
layout: section
---

# Going Production

---

# Try Going Production?
From the activity, you're still on DEBUG.

Try turning off `DEBUG`, do you see problems, why?

In many cases, going production for the first time creates issues and can be difficult to resolve.
That is the exact reason why most (web) frameworks, has checklist/manual for deploying applications.

See [Django's checklist](https://docs.djangoproject.com/en/5.1/howto/deployment/checklist/)

We will also go through some common issues and how to deal with them.

---

## Serving Static Files
You will most likely encounter this problem. When Django's `runserver` is on production, it will **not** serve static files automatically. There are many ways to fix this, here are some:

* Using a production-ready webserver and put the static files in place you want to serve the static files.
  
  You will set the `STATIC_ROOT` as a the directory where the webserver can point to and your files exist.

* Use external storage like CDNs or Buckets to store and serve static files.

* Use third-party library to manage static files for you, like [`WhiteNoise`](https://whitenoise.readthedocs.io/en/stable/index.html).

---

## `ALLOWED_HOSTS` Problem
When in production, be sure to set `ALLOWED_HOSTS` to include a correct name as an entry to the site.

Do not set to `["*"]` as it allows any other host to impersonate as your application.

---

## CORS Problem
When in production, be sure to correctly configure CORS in backend,
allowing frontend with the correct host to access the site.

It should not be set to `*` as it will allow anyone to use your backend.

---

## HTTPS
If you can have your site in HTTPS, great!

For Django applications, be sure to set `CSRF_COOKIE_SECURE` and `SESSION_COOKIE_SECURE` to `True` to prevent
sending cookies over HTTP accidentally.
