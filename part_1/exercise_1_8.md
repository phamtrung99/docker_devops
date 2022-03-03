## Topic 
![Topic_1_8_1](../public/part_1/image/Topic_1_8_1.png) 
![Topic_1_8_2](../public/part_1/image/Topic_1_8_2.png) 

## My answer
#### Step
1. First, create `Dockerfile` with content:
```
FROM ubuntu:20.04
WORKDIR /usr/src/app
COPY web-script.sh .
RUN apt-get update
RUN apt-get install -y curl
RUN chmod +x web-script.sh
CMD ./web-script.sh
```
2. Create `web-script.sh` with content:
```
echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;
```

3. Docker build
```
docker build . -t trung-curler
```

4. Run image
```
docker run -it trung-curler
```

#### Result
![Answer_1_8](../public/part_1/image/Answer_1_8.png)

