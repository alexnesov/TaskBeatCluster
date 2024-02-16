# Load deployments and services into Tilt
k8s_yaml([
  'k8s-manifests/fastapi-deployment.yaml',
  'k8s-manifests/fastapi-service.yaml',
  'k8s-manifests/react-deployment.yaml',
  'k8s-manifests/react-service.yaml'
])

# Define docker images
docker_build('fastapi-service', 'fastapi-service')
docker_build('react-service', 'react-service')
