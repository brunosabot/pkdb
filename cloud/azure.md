# Azure

## Contents

 - [Connect and push to Azure Container Registry](#connect_acr)

## <a name="connect_acr"></a>Connect and push to Azure Container Registry

Considering:
 - my registry is named `my-container-registry`.
 - my namespace is `my-ns`
 - my container is `my-docker-image`

```shell
az acr login --name my-container-registry
docker build . -t my-docker-image
docker tag my-docker-image my-container-registry.azurecr.io/my-ns/my-docker-image
docker push my-container-registry.azurecr.io/my-ns/my-docker-image
```
