# k8s-mongo
1. Create secrets
   ```
   kubectl create secret generic my-mongo-secret \
   --from-literal="MONGO_INITDB_ROOT_USERNAME=admin" \
   --from-literal="MONGO_INITDB_ROOT_PASSWORD=password"
   ```
2. 

