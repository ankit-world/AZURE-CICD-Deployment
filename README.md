# AZURE-CICD-Deployment-with-Github-Actions
Container Registries
    - create with resource group name and registry name
    -go to resources>access keys> save login url and password(once enabled)

## Save pass:

password you got from azure


## Run from terminal:

docker build -t simpleflaskapps.azurecr.io/flaskapps:latest .

docker login simpleflaskapps.azurecr.io

docker push simpleflaskapps.azurecr.io/flaskapps:latest


## Deployment Steps:

1. Build the Docker image of the Source Code
2. Push the Docker image to Container Registry
3. Launch the Web App Server in Azure 
4. Pull the Docker image from the container registry to Web App server and run 