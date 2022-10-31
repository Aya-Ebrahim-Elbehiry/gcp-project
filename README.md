# to build infra on gcp using terraform do : 


cd gcpProject/

terraform init

terraform apply

# to build image from docker file use :

docker build -t python-app .
docker tag python-app gcr.io/<iti-1-366311/python-app
docker push gcr.io/iti-1-366311/python-app
  
# to deploy the application on gke cluser 
  
 kubectl apply -f python-deployment.yaml
