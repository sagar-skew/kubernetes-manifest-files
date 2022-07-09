# kubernetes-manifest-files

kubectl get deployments
kubectl scale --replicas=3 deployment nginx-deployment


deployment rollout
kubectl set image deployment.v1.apps/nginx-deployment nginx=nginx:1.9.1 --record
kubectl rollout status deployment.v1.apps/nginx-deployment
kubectl rollout history deployment nginx-deployment


deployment rollback 
kubectl rollout undo deployments nginx-deployment
kubectl rollout history deployment nginx-deployment
kubectl rollout history deployment/nginx-deployment --revision=3
