kubectl apply -f <link to yaml> <br/>
kubectl -n kubernetes-dashboard create token kubernetes-dashboard <br/>
kubectl proxy<br/>
<br/>

weave
kubectl apply -f <linkt to yaml> <br/>
kubectl port-forward -n weave "$(kubectl get -n weave pod --selector=weave-scope-component=app -o jsonpath='{.items..metadata.name}')" 4040 <br/>
