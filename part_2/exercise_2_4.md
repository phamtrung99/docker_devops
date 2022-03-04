## Topic 
![Topic_2_4](../public/part_2/image/Topic_2_4.png) 

## My answer
#### Step
1. Create `docker-compose.yml` with content
```
version: "3.9"

services:
 example-frontend:
  image: example-frontend-trung
  depends_on:
   - example-backend
  ports:
   - "5001:5000"

 example-backend:
  image: example-backend
  environment:
   - REDIS_HOST=redis
  depends_on:
   - redis
  ports:
   - "8080:8080"

 redis:
  image: redis
  restart: unless-stopped
```

2. Run `docker-compose up`

#### Result
![Answer_2_4](../public/part_2/image/Answer_2_4.png)

