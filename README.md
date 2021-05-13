# django_blog

`api` — backend application

`build` — build scripts, docker/docker-compose


### Data Structure

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

### Endpoints

<table id="supsystic-table-19" data-border-spacing="" class="supsystic-table border lightboxImg cell-border dataTable no-footer" data-id="19" data-view-id="19_12230" data-title="resource ‘post’ Django REST Framework" data-currency-format="$1,000.00" data-percent-format="10.00%" data-date-format="DD.MM.YYYY" data-time-format="HH:mm" data-features="[&quot;after_table_loaded_script&quot;]" data-search-value="" data-lightbox-img="" data-head-rows-count="1" data-pagination-length="50,100,All" data-auto-index="off" data-searching-settings="{&quot;columnSearchPosition&quot;:&quot;bottom&quot;,&quot;minChars&quot;:&quot;0&quot;}" data-lang="default" data-override="{&quot;emptyTable&quot;:&quot;&quot;,&quot;info&quot;:&quot;&quot;,&quot;infoEmpty&quot;:&quot;&quot;,&quot;infoFiltered&quot;:&quot;&quot;,&quot;lengthMenu&quot;:&quot;&quot;,&quot;search&quot;:&quot;&quot;,&quot;zeroRecords&quot;:&quot;&quot;,&quot;exportLabel&quot;:&quot;&quot;,&quot;file&quot;:&quot;default&quot;}" data-merged="[]" data-responsive-mode="0" data-from-history="0" style="width:100%;" role="grid"><thead><tr role="row"><th class="" style="width:25%;padding:0 !important;" rowspan="1" colspan="1" data-original-value="" data-order=""></th><th class="" style="width:25%;padding:0 !important;" rowspan="1" colspan="1" data-original-value="" data-order=""></th><th class="" style="width:25%;padding:0 !important;" rowspan="1" colspan="1" data-original-value="" data-order=""></th><th class="" style="width:25%;padding:0 !important;" rowspan="1" colspan="1" data-original-value="" data-order=""></th></tr></thead><tbody><tr role="row" class="odd"><td data-cell-id="A1" data-x="0" data-y="1" class="bg-aeb3ac" data-cell-type="text" data-original-value="Endpoint" data-order="Endpoint" style="min-width: 25%; background-color: rgb(174, 179, 172);">Endpoint</td><td data-cell-id="B1" data-x="1" data-y="1" class="bg-aeb3ac" data-cell-type="text" data-original-value="HTTP Method" data-order="HTTP Method" style="min-width: 25%; background-color: rgb(174, 179, 172);">HTTP Method</td><td data-cell-id="C1" data-x="2" data-y="1" class="bg-aeb3ac" data-cell-type="text" data-original-value="CRUD Method" data-order="CRUD Method" style="min-width: 25%; background-color: rgb(174, 179, 172);">CRUD Method</td><td data-cell-id="D1" data-x="3" data-y="1" class="bg-aeb3ac" data-cell-type="text" data-original-value="Result" data-order="Result" style="min-width: 25%; background-color: rgb(174, 179, 172);">Result</td></tr><tr role="row" class="even"><td data-cell-id="A2" data-x="0" data-y="2" class="" data-cell-type="text" data-original-value="posts/" data-order="posts/">posts/</td><td data-cell-id="B2" data-x="1" data-y="2" class="" data-cell-type="text" data-original-value="GET" data-order="GET">GET</td><td data-cell-id="C2" data-x="2" data-y="2" class="" data-cell-type="text" data-original-value="READ" data-order="READ">READ</td><td data-cell-id="D2" data-x="3" data-y="2" class="" data-cell-type="text" data-original-value="Get all posts" data-order="Get all posts">Get all posts</td></tr><tr role="row" class="odd"><td data-cell-id="A3" data-x="0" data-y="3" class="" data-cell-type="text" data-original-value="posts/" data-order="posts/">posts/</td><td data-cell-id="B3" data-x="1" data-y="3" class="" data-cell-type="text" data-original-value="POST" data-order="POST">POST</td><td data-cell-id="C3" data-x="2" data-y="3" class="" data-cell-type="text" data-original-value="CREATE" data-order="CREATE">CREATE</td><td data-cell-id="D3" data-x="3" data-y="3" class="" data-cell-type="text" data-original-value="Create new post" data-order="Create new post">Create new post</td></tr><tr role="row" class="even"><td data-cell-id="A4" data-x="0" data-y="4" class="" data-cell-type="text" data-original-value="posts/:id" data-order="posts/:id">posts/:id</td><td data-cell-id="B4" data-x="1" data-y="4" class="" data-cell-type="text" data-original-value="GET" data-order="GET">GET</td><td data-cell-id="C4" data-x="2" data-y="4" class="" data-cell-type="text" data-original-value="READ" data-order="READ">READ</td><td data-cell-id="D4" data-x="3" data-y="4" class="" data-cell-type="text" data-original-value="Get post details" data-order="Get post details">Get post details</td></tr><tr role="row" class="odd"><td data-cell-id="A5" data-x="0" data-y="5" class="" data-cell-type="text" data-original-value="posts/:id" data-order="posts/:id">posts/:id</td><td data-cell-id="B5" data-x="1" data-y="5" class="" data-cell-type="text" data-original-value="PUT" data-order="PUT">PUT</td><td data-cell-id="C5" data-x="2" data-y="5" class="" data-cell-type="text" data-original-value="UPDATE" data-order="UPDATE">UPDATE</td><td data-cell-id="D5" data-x="3" data-y="5" class="" data-cell-type="text" data-original-value="Update post" data-order="Update post">Update post</td></tr><tr role="row" class="even"><td data-cell-id="A6" data-x="0" data-y="6" class="" data-cell-type="text" data-original-value="posts/:id" data-order="posts/:id">posts/:id</td><td data-cell-id="B6" data-x="1" data-y="6" class="" data-cell-type="text" data-original-value="PATCH" data-order="PATCH">PATCH</td><td data-cell-id="C6" data-x="2" data-y="6" class="" data-cell-type="text" data-original-value="UPDATE" data-order="UPDATE">UPDATE</td><td data-cell-id="D6" data-x="3" data-y="6" class="" data-cell-type="text" data-original-value="Partial update of post" data-order="Partial update of post">Partial update of post</td></tr><tr role="row" class="odd"><td data-cell-id="A7" data-x="0" data-y="7" class="" data-cell-type="text" data-original-value="posts/:id" data-order="posts/:id">posts/:id</td><td data-cell-id="B7" data-x="1" data-y="7" class="" data-cell-type="text" data-original-value="DELETE" data-order="DELETE">DELETE</td><td data-cell-id="C7" data-x="2" data-y="7" class="" data-cell-type="text" data-original-value="DELETE" data-order="DELETE">DELETE</td><td data-cell-id="D7" data-x="3" data-y="7" class="" data-cell-type="text" data-original-value="Delete post" data-order="Delete post">Delete post</td></tr><tr role="row" class="even"><td data-cell-id="A8" data-x="0" data-y="8" class="" data-cell-type="text" data-original-value="posts/:id" data-order="posts/:id">posts/:id</td><td data-cell-id="B8" data-x="1" data-y="8" class="" data-cell-type="text" data-original-value="OPTIONS" data-order="OPTIONS">OPTIONS</td><td data-cell-id="C8" data-x="2" data-y="8" class="" data-cell-type="text" data-original-value="" data-order=""></td><td data-cell-id="D8" data-x="3" data-y="8" class="" data-cell-type="text" data-original-value="Return supported HTTP methods" data-order="Return supported HTTP methods">Return supported HTTP methods</td></tr></tbody><style>#supsystic-table-19.oneColumnWithLabels td:nth-of-type(1):before { content: ""; }#supsystic-table-19.oneColumnWithLabels td:nth-of-type(2):before { content: ""; }#supsystic-table-19.oneColumnWithLabels td:nth-of-type(3):before { content: ""; }#supsystic-table-19.oneColumnWithLabels td:nth-of-type(4):before { content: ""; }</style></table>


### How to run

#### Development mode

`docker-compose -f build/docker-compose-dev.yml up`

will run only services needed for development like PostgreSQL, Redis etc

`docker-compose -f build/docker-compose-api.yml up`

will run all needed services and API (backend application)
