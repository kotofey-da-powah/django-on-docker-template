# Django on Docker Template

This is ready-to-run Docker template with **Django + Postgres + Redis + Gunicorn + Nginx**

![Django on Docker](https://cdn.filestackcontent.com/rJf1U9MTraWZDCJWjQoE)

## Quick start

```shell script
git clone https://github.com/kotofey-da-powah/docker-on-django-template
cd docker-on-django-template
cp backend/.env.template backend/.env

docker-compose up -d --build
```

Open `http://localhost` and you're done!

----------------------------------
To run Gunicorn + Nginx type:
```shell script
docker-compose -f docker-compose.prod.yml up -d --build
```

## Overview

This project contains docker-compose configurations with:

* Django
* Postgres
* Redis _(optional / commented)_
* Gunicorn and Nginx _(docker-compose.prod.yml)_

File `backend/.env.template` contains example environment variables
which needs for project set up. Docker-compose looks up for **`backend/.env`** file.

