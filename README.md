# Learning Roadmap: Kubernetes

Curso: https://www.udemy.com/course/learn-devops-the-complete-kubernetes-course

## Modulo 1

Objetivos: 

- Instalar Cluster Local (En windows: Docker for Desktop + WSL)
- Desplegar un servicio básico dockerizado localmente y accederlo mediante HTTP
- Crear un cluster remoto en algun proveedor cloud (el curso usa AWS y kops, yo use GKE directamente)
- Desplegar el mismo servicio dockerizado, exponerlo, y accederlo mediante HTTP


## GKE

- Primero crear una cuenta en GKE usando el free tier
- Luego instale y configure [Gcloud CLI](https://cloud.google.com/sdk/docs/install)
- Cree un cluster mediante Gcloud CLI: `gcloud container clusters create cluster-1 --zone us-central1-c --project learn-k8s-123`

Con todo instalado, se puede mirar los clusters a los que estamos conectados usando:

`kubectl config get-contexts`

Y cambiar el cluster usando:
`kubectl config use-context <NOMBRE DEL CONTEXT>`