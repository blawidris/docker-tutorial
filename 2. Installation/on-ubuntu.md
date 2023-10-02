
## Installation on Ubuntu

**Step 1:** follow the following link
- https://docs.docker.com/desktop/install/ubuntu/
- https://docs.docker.com/engine/install/ubuntu/#set-up-the-repository

**Step 3:** Verify that the Docker Engine installation is successful

```

// check composer version

docker compose version

// check docker version
docker --version

// running a hello-world image

sudo docker run hello-world

```

**Step 4:** Lauch Docker Desktop

```systemctl --user start docker-desktop
```

**Step 5:** Stop Docker Desktop

``` 
systemctl --user stop docker-desktop
```

#### To enable Docker Desktop to start on login

``` systemctl --user enable docker-desktop ```
