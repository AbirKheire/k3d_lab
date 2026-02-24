# k3d_lab

## 📌 Objectif du TP

Automatiser avec Ansible :

- La création d’un cluster Kubernetes léger avec k3d
- Le déploiement d’un service NGINX
- L’exposition du service en NodePort

Ce TP permet de comprendre l’automatisation d’un environnement Kubernetes local.

---

## ⚙️ Prérequis

- Linux / WSL Ubuntu
- Docker Desktop installé et fonctionnel
- Ansible installé

Vérifier Docker :

```bash
docker info
```

---

## ▶️ Lancer le rôle

Depuis la racine du projet :

```bash
ansible-playbook -i localhost, playbooks/ansible-role-k3d-lab.yaml
```

---

## 🌍 Accès au site

Après exécution :

```
http://localhost:30080
```

---

## 🔧 Variables

| Variable            | Valeur par défaut |
|---------------------|------------------|
| k3d_cluster_name    | k3d-lab          |
| k3d_nodeport        | 30080            |
