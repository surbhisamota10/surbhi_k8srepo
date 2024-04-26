Why kubernetes???

Docker drawback 

1) single host in a docker on a single host we install docker and on that docker we create 100 container and all 100 container used resources from a single host if 80
containers will take high resources then one of the container will die or process will destroy due to other taking high resources .

2) lets say someone killed one of the container then application will not accessible  and there are so many reason due to which conatiner will stopped in production there are thousands of
containers used and 100;s of resaon due to which conatiner will stop so we cannt handle it.
But there is auto healing property k8s have.

3) lets say your container has capacity of 4 GB RAM and 2 core CPU and your application(ecommerce) handles 1000 users but on festival season users will incresase with 20000 or more than 
application down now you want to create manually container and also need to apply load balancing
but in k8s there is auto scaling property.

4) bydefault docker doesn't have enterprise level support 

******************************************************************************************************************************************************************************************

Cluster is a group of nodes
node ===server===docker host
pod=== (container's cover) === label of conatiner
without container your pod is nothing 
cluster not communicate with container it communicate with pod.


*******************************************************************************************************************************************************************************************

K8S advantage

1) k8s fix the single host problem if there is a pod down due to load or high resources taking by other then k8s auto. shift on another node

2) Auto healing : API server heals the posd

3) Auto scaling : handles buy replica set

4) k8s have enterprise level support.
