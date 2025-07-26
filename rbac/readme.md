--> to crete the role and role binding use the role.yaml and rolebinding.yaml
--> and to set the set-credentials
kubectl config set-credentials <name> \
  --client-certificate=<name>.crt \
  --client-key=<name>.key


-> to set the context to the cluster
kubectl config set-context admin --cluster=<cluster name> --user=<user name "adam">