# TP 33 : Déploiement d’une application Spring Boot sur Kubernetes

## 🎯 Objectifs pédagogiques

À la fin de ce TP, vous serez capable de :

- Conteneuriser une application **Spring Boot** avec **Docker**.
- Créer les manifests Kubernetes de base : **Deployment** et **Service**.
- Déployer l’application sur un **cluster Kubernetes local** (Minikube, kind, k3d…).
- Exposer l’API Spring Boot vers l’extérieur du cluster via un **Service de type NodePort**.
- Vérifier le fonctionnement et observer les **pods** dans le cluster.

---
<img width="1868" height="938" alt="image" src="https://github.com/user-attachments/assets/dd9cddcc-4237-4617-b83e-85dfb1f65392" />

## 🧩 Scénario

On dispose d’une petite API REST Spring Boot qui expose un endpoint :

- `GET /api/hello`  
  → retourne un message JSON du type :

```json
{
  "message": "Hello from Spring Boot on Kubernetes!"
}




