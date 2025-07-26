
to creaet service account 
 use the secret.yaml file

--> to creaet role 
kubectl create role build-role \
> --verb=list,get,watch \
> --resource=pod
role.rbac.authorization.k8s.io/build-role created

--> to create rolebinding
