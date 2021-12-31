# kubernetes-beginner- Lab 00- Kubernetes Setup
 ## Q1) How many nodes are part of the cluster?
    Ans: kubectl get nodes
 ## Q2) What is the version of Kubernetes running on the nodes?
    Ans: kubectl version
 ## Q3) What is the flavour and version of Operating System on which the Kubernetes nodes are running
    Ans: kubectl get nodes -o wide

# kubernetes-beginner- Lab 01- Pods With YAML
 ## Q1) How Many pods exist on the system? 
    Ans: kubectl get nodes
 ## Q2) Create a new pod with the nginx image.
    Ans: kubectl run nginx --image=nginx
 ## Q3) What is the image used to create the new pods?
 ## You must look at one of the new pods in detail to figure this out.
    Ans: kubectl describe pod podName-bcmv4 | grep -i image
 ## Q4) Delete webapp pod?
    Ans: kubectl delete pod webapp
 ## Q5) Create a new pod with the name redis and with the image redis123.
 ## Use a pod-definition YAML file. And yes the image name is wrong!
    Ans: kubectl run redis --image=redis123
