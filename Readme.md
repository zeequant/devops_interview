# DevOps Interview

#### Given
- You will be given kubernetes cluster with a single node with 2 CPU 2 GB Ram.
- The clusters configuration file will be given to you.
- This repository has 2 node servers(using express js)

Step 1
Create docker file for service_1. Publish to docker hub.
Deploy the docker image to the provided kubernetes cluster.
And you should be able to open the service deployed in kubernetes from
you local machine browser using a public ip/url.


Step 2
Create docker file for service_2. Publish to docker hub and deploy to cluster.
Using nginx, reverse proxy, if url is `/1/` then proxy to service 1 at `/`
Using nginx, reverse proxy, if url is `/2/` then proxy to service 2 at `/`

Step 3
Create a postgresql database using helm charts and deploy cluster.
Create docker file for service_3 and deploy it by sending POSTGRESQL_URL env var
containing the url for that database.
Using nginx, reverse proxy, if url is `/3/` then proxy to service 3 at `/`
