1. Create a volume
```
docker volume create myvol
```
2. List volumes
```
docker volume ls
```
3. Run bash in container
```
docker run --rm -it -v myvol:/app ubuntu bash
```
4. Create a file in volume
```
touch /app/file
```
4. Exit container
5. Create container from point 3
6. List files in `/app`
```
ls /app
```
7. Exit container and remove volume
```
docker volume rm myvol
```
8. Create a block in memory
```
docker run --rm -it --tmpfs /app ubuntu bash 
```
8. Create 1 GB file
```
dd if=/dev/zero of=/app/test bs=1k count=1000000
```
9. In host console monitor memory usage
10. Run bash from container and list `/user` directory
```
docker run --rm -it -v "/home/<USER_NAME>:/user" ubuntu bash
```