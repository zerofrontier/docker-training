1. Run pgadmin in container
```
docker run -p 80:80 -e "PGADMIN_DEFAULT_EMAIL=admin" -e "PGADMIN_DEFAULT_PASSWORD=asdasd" dpage/pgadmin4

```
3. Try to access console from person next to you
3. Run pgadmin in container in proper way
```
docker run -p 127.0.0.1:80:80 -e "PGADMIN_DEFAULT_EMAIL=admin" -e "PGADMIN_DEFAULT_PASSWORD=asdasd" dpage/pgadmin4

```