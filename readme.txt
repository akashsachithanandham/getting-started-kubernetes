Steps to run the Hello world application in Kubernetes locally:

Step 1: create a folder for flask application
Step 2: make a hello world application using flask
step 3: install the docker to containerize the python app
step 4: go inside to your current project folder
        cd getting-started/app
step 5: build the app using 
        sudo docker build -t getting-started-app .

step 6: after building the app run it.
        sudo docker run  -p 5000:5000 getting-started-app
step 7: Now containerization is done.Next we have go for Kubernetes.

step 8: install Kubernetes locally 

step 9: install minikube to run in single node cluster

Some terminologies:
Cluster: a clustter is the large one which contains more nodes 
Nodes: Node is a smallest computational components (ex our computer,hardware components)
Pod: A Pod is there inside the nodes and contains many containers. A pod is used for replication and load balancing.
Container: A Container can be the smallest one which contains our application.


Commands to run Kubernetes:

1. start the minikube
 minikube start
2. build the yaml file and apply it
 kubectl apply -f deployment.yaml
3. to see the no of replications and available pods for the containers
 kubectl get pods
4. to see the service list and to get the host and port
 minikube service list
