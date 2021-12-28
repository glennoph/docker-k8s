# simplek8s 
## files
* client-pod.yaml - pod, container for image stephengrider/multi-client
* client-node-port.yaml - service NodePort for multi-client
## Commands
### start
`kubectl apply -f client-pod.yaml`
* start client-pod
`kubectl apply -f client-node-port.yaml`
* start service
### list
`kubectl get pods`
* name: client-pod
`kubectl get services`
* name: client-node-port
### delete

`kubectl delete pod client-pod`
* pod "client-pod" deleted

`kubectl delete service client-node-port`
* service "client-node-port" deleted
