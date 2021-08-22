Link to Github: https://github.com/trancongminh997-hub/de_homework

Link to Docker hub: https://hub.docker.com/r/trancongminh997/sorting_api

### API
```
http://<host>:5000/sorting
Methods: POST
JSON: ex: {"data": [11, 2, 99], "order": 'asc'}
Description: return a sorted list
```

### To run as a container:
```
# Run a new container
docker run --rm -it -p 5000:5000 --name ins1 trancongminh997/sorting_api

# Check for functional test
docker exec -it ins1 sh -c "python test_services.py"
```