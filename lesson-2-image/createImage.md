1. Run bash in container
```
docker run -it ubuntu bash
```
2. Modify it
```
apt-get update
apt-get install -y figlet
figlet "hello, world!"
```
3. Exit bash
4. Find container ID
```
docker container ls -a
```
5. Commit container
```
docker container commit <CONTAINER_ID>
```
6. List images
```
docker image ls
```
7. tag a new image
```
docker image tag <IMAGE_ID> firstimage
```
8. Run image
```
docker run firstimage figlet hello
```
9. Build ready image
```
docker image build -t hello .
```
10. Run second image
```
docker run firstimage figlet hello
```