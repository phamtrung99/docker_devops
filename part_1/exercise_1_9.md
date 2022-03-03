## Topic 
![Topic_1_9](../public/part_1/image/Topic_1_9.png) 

## My answer
#### Step
1. Run image with command
```
docker run -v "$(pwd)/log/applog.txt:/usr/src/app/text.log" devopsdockeruh/simple-web-service:alpine
```
Its mean we want to mount the file in container `/usr/src/app/text.log` to outside, in my computer directory is `/log/applog/.txt`.

#### Result
![Answer_1_9](../public/part_1/image/Answer_1_9.png)

