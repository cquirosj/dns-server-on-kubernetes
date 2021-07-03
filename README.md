DNS server in a container hosted in kubernetes

The solution consists of one deployment and two services:

- The deployment is the one that creates a pod with the container
- The first service exposes an ip address to access the UI. While visiting the UI use as user and password the word update. These values are configured in the deployment.yaml file as environment variables to the container.
- The second service exposes another ip address to be used by the clients as the DNS server.