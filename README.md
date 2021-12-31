# install docker in jenkins container
```
docker exec -it --user root <container id> bash
```
Then
```
curl https://get.docker.com/ > dockerinstall && chmod 777 dockerinstall && ./dockerinstall
```

Exit out of the Jenkins container interactive shell, and run the following command to change permissions on “docker.sock” for added security
```
sudo chmod 666 /var/run/docker.sock
```


