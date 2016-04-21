# Jetbrains Youtrack
Docker image: Alpine Linux 3.3- openJAVA JRE 8- Jetrbains Youtrack 6.5

[YouTrack](https://jetbrains.com/youtrack/) is an issue tracking and project management tool from [JetBrains](https://jetbrains.com/).


## Usage

Pull the image, create a new container and start it:

```bash
docker pull boutch/youtrack
docker create --name youtrack -p 8080:8080 --restart=always boutch/youtrack
docker start youtrack
```

Mount your data in volumes:

```bash
docker pull boutch/youtrack
docker create --name youtrack -p 8080:8080 -v /srv/youtrack:/var/lib/youtrack --restart=always boutch/youtrack
docker start youtrack
```


