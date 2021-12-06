For this we are using minikube.

What is minikube :
    Basically a light version of k8s , for testing or lightweight work , can be used in production 
    although not recommended (requires lots of configuration).

    Github link : https://github.com/kubernetes/minikube


1 Step : Starting 

   Insatllation steps i'm skiping as it can easily be found on website , and are different for diff 
   platform.

<code>minikube version</code> (for version checking || for checking succesful insatllation)

<code>minikube start --wait=false</code> (Starting cluster)

2  Step : Getting cluster info

   <code>kubectl cluster-info</code> ( kubectl is cli for k8s)

   <code>kubectl get nodes</code>  (for getting active nodes information)

We may as , What are nodes ?? 
    Basically smallest vm kinda unit that are controlled by vm using vm server , proxies and networking.
    Each nodes can have one or more pods , pods are individual workloads same like a docker instance.

status tab show status , if it say ready then our pod is ready to use.

3 step : Deploy Containers
    <code>kubectl create deployment first-deployment --image=<any image ></code>

    This is for creating a deployment ( for launching instance)

    <code>kubectl get pods</code> see if the pods are ready?

    Now even the containers are ready , they have to be exposed to exposed to outside world as they still
    run under k8s.

    Possible solutions are.
    cluster-ip
    nodeport
    loadbalancer
    externalName

    Quick summary of them :
    They all are services for letting our pods communicate to each other:

    -> cluster-ip is only for internal communication and is default option
    -> nodeport used when we need to access cluster-ip from outside too.
    -> loadbalancer , load balance between all external ip of pods.
    -> externalName (not clear now).

4 step : Accessing dashboard.

    <code>minikube addons enable dashboard</code>

    and apply the settings for dashboard(yaml file can be found on internet).

And done.


We learned to start a mini cluster , deploy app and Accessing dashboard.



