<!-- TITLE: Command Line -->
<!-- SUBTITLE: A quick summary of Command Line -->

# Command line


```text
docker container ls
docker container top nginx
docker container inspect nginx
docker container stats --help
docker container stats
```



-----


```
docker container run -it   (start new container interactively)
docker container exec -it   (run additional command in existing container)
docker container run -it --name proxy nginx bash
docker container start --help
docker container start -ai ubuntu
```

-----


**Docker Network**
```
docker container run -p
docker container port <container>

```
