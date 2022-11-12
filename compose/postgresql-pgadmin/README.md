# PostgreSQL with pgAdmin

> ## PostgreSQL
> PostgreSQL is a powerful, open source object-relational database system.
> - Image: https://hub.docker.com/_/postgres

> ## pgAdmin
> pgAdmin is the most popular and feature rich Open Source administration and development platform for PostgreSQL.
> - Image: https://hub.docker.com/r/dpage/pgadmin4
> - Documentation: https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html
---
## How to (steps 1 and 2 only if default envs dont fit your needs):
1. Duplicate .env.example and rename the copy to be '.env'
2. Specify env variables in .env file (_if defaults are not sufficient_)
3. Run ```docker compose up``` in this directory
4. Find pgAdmin at [localhost:5050](http://localhost:5050/), or _localhost:<PGA_PORT>_ if you changed the port in .env
5. Connect to PostgreSQL instance at _postgres:5432_ or _postgres:<PG_PORT>_ from pgAdmin, or at [localhost:5432](http://localhost:5050/) or _localhost:<PG_PORT>_ from your docker host  
Use the username, password, port and db-name specified for PostgreSQL to connect, hostname is _postgres_ (name of the container network)