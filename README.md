# django_blog

`api` — backend application

`build` — build scripts, docker/docker-compose

## Data Structure

```
├── api
│   ├── django_blog
│   │   ├── apps
│   │   │   ├── account
│   │   │   │   ├── admin.py
│   │   │   │   ├── apps.py
│   │   │   │   ├── forms.py
│   │   │   │   ├── __init__.py
│   │   │   │   ├── managers.py
│   │   │   │   ├── migrations
│   │   │   │   │   ├── 0001_initial.py
│   │   │   │   │   └── __init__.py
│   │   │   │   └── models.py
│   │   │   ├── common
│   │   │   │   ├── apps.py
│   │   │   │   ├── __init__.py
│   │   │   │   ├── management
│   │   │   │   │   ├── commands
│   │   │   │   │   │   ├── generate_secretkey.py
│   │   │   │   │   │   ├── __init__.py
│   │   │   │   │   │   └── startapp.py
│   │   │   │   │   └── __init__.py
│   │   │   │   └── models
│   │   │   │       ├── core.py
│   │   │   │       └── __init__.py
│   │   │   └── __init__.py
│   │   ├── __init__.py
│   │   ├── settings
│   │   │   ├── contrib.py
│   │   │   ├── django_blog.py
│   │   │   ├── django.py
│   │   │   ├── environment.py
│   │   │   └── __init__.py
│   │   ├── urls.py
│   │   └── wsgi.py
│   ├── Makefile
│   ├── manage.py
│   ├── pylama.ini
│   ├── pyproject.toml
│   ├── pytest.ini
│   └── requirements
│       ├── common.in
│       ├── common.txt
│       ├── dev.in
│       └── dev.txt
├── build
│   ├── ci
│   │   └── circle.yml
│   ├── docker-compose-api.yml
│   ├── docker-compose-dev.yml
│   ├── docker-entrypoint-api.sh
│   └── Dockerfile.api
├── circle.yml -> build/ci/circle.yml
└── README.md
```

### How to run

#### Development mode

`docker-compose -f build/docker-compose-dev.yml up`

will run only services needed for development like PostgreSQL, Redis etc

`docker-compose -f build/docker-compose-api.yml up`

will run all needed services and API (backend application)
