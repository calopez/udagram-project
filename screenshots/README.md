# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::
## Working Application
<img width="1677" alt="Screen Shot 2021-11-28 at 12 18 41" src="https://user-images.githubusercontent.com/3010579/143778777-de06221c-01e6-4b99-b420-fe87b001c82c.png">

## Deployment Pipeline
* DockerHub showing containers that you have pushed
<img width="420" alt="docker-hub-repositories" src="https://user-images.githubusercontent.com/3010579/143776807-0d534520-07b9-4008-84e9-b46422da7791.png">
e.g.
<img width="418" alt="dockerhub-udagram-api-feed" src="https://user-images.githubusercontent.com/3010579/143776833-cf0e804a-3efc-4f54-a80a-c9701488a05b.png">

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
<img width="934" alt="Screen Shot 2021-11-28 at 11 46 55" src="https://user-images.githubusercontent.com/3010579/143777719-269a982b-9be0-4f16-a986-c8ae708e5181.png">

* Travis CI showing a successful build and deploy job
<img width="840" alt="travis-CI" src="https://user-images.githubusercontent.com/3010579/143777725-76ebf8dd-3063-4b80-8019-2692bfed56e7.png">

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
<img width="684" alt="kubectl-get-pods" src="https://user-images.githubusercontent.com/3010579/143777783-3830ca6b-2d96-43e1-88f0-9a09edd7bce8.png">

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
<img width="792" alt="kubectl-describe-services-I" src="https://user-images.githubusercontent.com/3010579/143777822-5fcdb29b-e6a7-4b91-85c8-bb8cf39a2b0e.png">

<img width="401" alt="kubectl-describe-services-II" src="https://user-images.githubusercontent.com/3010579/143777824-c4a4f0d6-0b3c-427a-bdc7-df1e78bdffdb.png">

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
<img width="1912" alt="kubectl-describe-hpa-II" src="https://user-images.githubusercontent.com/3010579/146457971-afdf88b4-4e55-4415-8af7-1f089832657d.png">

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
<img width="1678" alt="Screen Shot 2021-11-28 at 12 12 52" src="https://user-images.githubusercontent.com/3010579/143778584-28dd05e3-8f18-4567-acbc-4d1be1a08df9.png">
