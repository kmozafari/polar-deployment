# polar-deploymant

## Kubernetes
### Polar-UI error in K8s deployment

https://github.com/keycloak/keycloak/discussions/22398

Run "minikube ip --profile polar" and add IP address to the /etc/hosts =>  IP polay-keyclock

## Docker

SPRING_SECURITY_OAUTH2_CLIENT_PROVIDER_KEYCLOAK_ISSUER_URI=http://polar-keycloak:8080/realms/PolarBookshop (work around by adding "127.0.0.1 polar-keycloak" to host /etc/hosts file)

SPRING_SECURITY_OAUTH2_RESOURCESERVER_JWT_ISSUER_URI=http://polar-keycloak:8080/realms/PolarBookshop
