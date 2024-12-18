# DevOps-Task-2

## Steps to run

1. Clone this repo `https://github.com/jayoswal/DevOps-Task-2.git`
2. Change directory to sample-helm-chart/
3. Execute command `helm install sample-helm-chart .`
4. Check pods are running using command `kubectl get pods`
5. Forward Kubernetes port through command `kubectl port-forward svc/backend-svc 8000:8000`

## Steps to test
1. Call GET API at (use postman)
>http://localhost:8000/

2. Check redis for moving hits `kubectl exec -it <redis-pod-name> -- redis-cli`
 i. Check hits value: `GET hits`
