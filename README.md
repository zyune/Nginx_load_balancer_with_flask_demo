# This is a small demo to implement load balance (round Robin) with nginx

### Please make sure your docker service is start in your machine.
### make sure the port 80 is not being occupied by any nginx process in your machine
To check that👆🏻， run ```lsof -i :80```
if there is use ```kill -9 PID```
### go to the root directory run following code, to start the container
```docker-compose up -d --build --scale app=3```

### Go to http://localhost:80/ , try to refresh the several time you can see the changes of container ID showing on your web browser
```
container ID: XXX
container ID: XXX
container ID: XXX
```
### If you want to stop the container use 
```docker-compose down```
