# a Pod is the smallest deployable unit of computing.Inside Pod generally we will have one container but it can be more as well.

# In a sidecar usecase, all similar containers should go to single pod to manage the scaling easily.

      => In a single pod all contaners share the shared netwrork and resources, which helps to spin the containers with ease.
      => This helps when delteting/creating new POD managing the pod becomes very easy (whatever a pod has we will delete/create all of the resources)
      => Each POD will have unique IP address and range of ports.
      => We can run same application of another instance with same port in different POD in same Node.This really cool when we scale application by incresing Pods based on Load
      => Inside a single pod , containers can communicate through local host.
      => Pod to Pod communication happens via IP address.

# To delete the pod kubectl delete pod `<podname>`
