# 🚀 K3s MyApp + PostgreSQL Deployment

Ovaj projekat prikazuje kako deploy-ovati jednostavnu aplikaciju (nginx) i PostgreSQL bazu u **K3s klasteru** pomoću YAML fajlova.

> ✅ Odličan primer za DevOps praksu, učenje Kubernetes-a i izgradnju portfolija.

---

## 🧱 Arhitektura

[ K3s Cluster ]
|
├── myapp (nginx)
| └── Service: NodePort (80 → host port)
|
└── postgres (PostgreSQL 15)
├── PVC (persistent volume)
└── Service: ClusterIP (5432)
