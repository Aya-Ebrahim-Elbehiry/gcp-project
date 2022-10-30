# to build infra on gcp using terraform do : 


cd gcpProject/

terraform init

terraform apply

# to build image from docker file use :

docker build -t <img-name> .
docker tag <img-name> gcr.io/<project-id>/<img-name>
docker push gcr.io/<project-id>/<img-name>
  
# to deploy the application on gke cluser 
  
 kubectl apply -f python-deployment.yaml
