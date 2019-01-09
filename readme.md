Start box1 and box2
```sh
docker-compose -f docker-compose.box1.yaml up -d
docker-compose -f docker-compose.box2.yaml up -d
```

Test box1 and box2 is on the same network
```sh
docker exec -it box2 sh

# In box2
ping box1
```