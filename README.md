# springboot-registration
A microservice to manage user registration data and details using postgresql database

To run a PostgreSQL using Docker, we first need to pull the postgres public image available on Docker Hub:

```bash
docker pull postgres
```

Now we'll run the Docker container using the postgres:latest image with the below command:

```bash
docker run --name marcomarco-postgres -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=secret -e POSTGRES_DB=user_registry -d -p 5432:5432 -v /tmp/postgres-data:/var/lib/postgresql/data postgres
```