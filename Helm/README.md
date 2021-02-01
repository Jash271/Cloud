# Creating Helm Chart for Kubernetes Application and Deploying it to Github Actions for Public Use

## Creating and Running Helm Charts Locally

### Creating a Helm Chart

```
helm create <name of the Application>
```

### Navigate to the Templates folder and Copy Paste Kubernetes Config File

### Install the Helm Chart Locally

```
helm install <name of chart >  <path to the Chart Folderm>
```

---

## Deploying Helm Chart for Public Use on Github Pages

### Create A Github Repository and Enable Github Pages

### Create Helm Chart Package

```
helm package <name of helm package folder>/*
```

### Create Index.yml File using this Command

```
helm repo index --url <your github pages url>
```

### A tar.gz zip file will be created

### Push to Github (Keep Root as target if tar.gz in Root Folder else if tar.gz in docs folder then docs should be set as target for Github Pages )

### Install and Run Your Helm Chart

```
helm install <github pages url for your helm zip folder >
```

### Example :

https://jash271.github.io/Test_helm/nodejsk8-helm-chart-0.1.0.tgz
