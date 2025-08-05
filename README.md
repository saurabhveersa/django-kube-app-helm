
---

## ✅ 1. `django-kube-app-helm/README.md`

```markdown
# Helm Chart: django-kube-app

This Helm chart deploys the Django application to Kubernetes with optional support for HPA and Ingress.

---

## 📁 Structure
django-kube-app-helm/
├── Chart.yaml
├── values.yaml
├── templates/
│ ├── deployment.yaml
│ ├── service.yaml
│ ├── ingress.yaml
│ ├── configmap.yaml
│ ├── hpa.yaml
│ └── keda-scaledobject.yaml
└── README.md


# Deploy Using Helm

helm upgrade --install django-kube-app ./django-kube-app-helm -n django-kube-ns

Or let Argo CD sync the app from the Git repo.

# Access Your App

Once deployed, and assuming DNS entry is set:

http://django-kube-app.local/api/management/?format=api



