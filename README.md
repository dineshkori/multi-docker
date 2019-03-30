# multi-docker
Multi Docker containers on Ngnix and react example

##### For Docker images build
docker build -t dkori/multi-client ./client
docker build -t dkori/multi-ngnix ./ngnix
docker build -t dkori/multi-server ./server
docker build -t dkori/multi-worker ./worker

##### Docker login to your Account
docker login

###### For Push 
docker push dkori/multi-client 
docker push dkori/multi-ngnix 
docker push dkori/multi-server 
docker push dkori/multi-worker