## Topic 
![Topic_2_2](../public/part_2/image/Topic_2_2.png) 

## My answer
#### Step
1. Create `docker-compose.yml` with content
```
version: '3.8'
services:
 simple-web:
  image: devopsdockeruh/simple-web-service
  build: .
  volumes:
   - ./log:/usr/src/app/text.log
  command: server
  container_name: simple-web
```

2. Run `docker-compose up`

