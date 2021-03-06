# Overview

This is template for Azure TFS pipeline for .NET Core microservice. View dockerfiles in [Dockerization template](https://github.com/pip-templates/pip-templates-microservice-dockerization).

# Usage

Copy component.json and *.ps1 scripts to microservice folder and import Build scripts (Azure.Example.CI.json and Azure.Microservice_build_tasks) and Release scripts (Azure.Example.Deploy and Azure.Microservice_release_tasks) to Azure TFS

# Settings

Required environment variables:
* **DOCKER_REGISTRY_SERVER** - docker registry server
* **DOCKER_USER** - docker username to access docker registry on image publish
* **DOCKER_PASS** - docker password to access docker registry on image publish


* **NUGET_SOURCE_NAME** - nuget source name
* **NUGET_SOURCE_URL** - docker source url
* **NUGET_USERNAME** - nuget username to access nuget repository on image publish
* **NUGET_PASSWORD** - nuget password to access nuget repository on image publish


* **K8S_CERTIFICATE_AUTHORITY_DATA** - kubernetes certificate authority data
* **K8S_SERVER** - kubernetes server
* **K8S_CLUSTER_NAME** - kubernetes cluster name
* **K8S_USER_NAME** - kubernetes username
* **K8S_CONTEXT_NAME** - kubernetes context name
* **K8S_CLIENT_CERTIFICATE_DATA** - kubernetes client certificate data
* **K8S_CLIENT_KEY_DATA1** - kubernetes client key first 50% data
* **K8S_CLIENT_KEY_DATA2** - kubernetes client key second 50% data
* **K8S_TOKEN** - kubernetes token
