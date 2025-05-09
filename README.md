## Installation

1. Clone the repository:
``` sh
git clone https://github.com/tyanfarm/seamless-streaming
```

2. Open folder: 
``` sh
cd seamless-streaming
```

3. Build docker image
``` sh
DOCKER_BUILDKIT=1 docker build -t seamless-app:latest .
```

4. Build docker container
``` sh
docker run --gpus all -p 7860:7860 --name seamless-container seamless-app:latest
```

5. Check logs
``` sh
docker logs -f seamless-container
```

The server will listen on port 7680 by default. 