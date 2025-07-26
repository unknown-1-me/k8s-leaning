->>to create the private key 
 openssl genrsa -out <name with .key> 2048

-->> to creaet csr cetficate 
openssl req -new -key <private key file name> -out my.csr -subj "/CN=admin"

-->> to creaete base64 plain text
cat <filename (my.csr)> | base64 | tr -d "\n"

->> to get the cetficat 
kubectl get csr

--> to aprove the certificate
 kubectl certificate approve <name of the cetficate>
