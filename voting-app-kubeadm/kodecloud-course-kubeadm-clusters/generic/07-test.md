# Test the cluster

Do the following on `controlplane`

[//]: # (host:controlplane)

1. Deploy the voting-app deployment and service

    ```bash
    cd /vagrant/voting-app
    kubectl create -f .
    ```

2.  Hit the new service
    Check the port of result and vote NodePort service using:

    ```bash
    kubectl get all
    ```

    The ports should be 31001 and 31000.

---

Do following on `web browser on windows`

1. Open your web browser on windows and access any of the <vm_ip>:<port_no>

    **Example :** 

    If controlplane IP is 192.168.0.112, open following in browser for result app: http://192.168.0.112:31001/

    You can access from any of the nodes, I have just used controlplane as an example.

---

Congratulations! You now have a working kubeadm cluster.


Prev: [Worker nodes](./06-workers.md)


