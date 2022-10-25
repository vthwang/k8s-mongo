# k8s-mongo
1. Create secrets
   ```
   kubectl create secret generic my-mongo-secret \
   --from-literal="MONGO_INITDB_ROOT_USERNAME=admin" \
   --from-literal="MONGO_INITDB_ROOT_PASSWORD=password"
   ```
2. Start mongo service.
   ```
   make dev
   ```
3. Connect to mongoDB.
   ```
   kubectl port-forward svc/my-mongo 27017:27017
   ```
