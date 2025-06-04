# Elastic Stack on Kubernetes

## Objective
Deploy the **Elastic Stack (Elasticsearch, Kibana, and Filebeat)** on a Kubernetes cluster using only YAML files (no Helm, no Operator).  
Filebeat is configured to collect logs from a sample application and send them to Elasticsearch.

---

## Project Structure
```
.
├── elasticsearch/   # Elasticsearch StatefulSet and Service YAML files
├── kibana/          # Kibana Deployment and Service YAML files
├── filebeat/        # Filebeat DaemonSet, ConfigMap, ServiceAccount, ClusterRole, ClusterRoleBinding
├── hello-world/     # Simple Hello World Pod (log source)
└── screenshots/     # Screenshots showing logs in Kibana and pod status
```

---

## Screenshots

- ✅ Kibana Discover showing logs from `hello-world` pod  
- ✅ `kubectl get pods` showing all components are running  
- ✅ Sample `Hello from Kubernetes!` log output from pod

---

## Result

Successfully deployed a working ELK stack with Filebeat on Kubernetes using only YAML files.  
Logs from the Hello World pod were collected by Filebeat and shown in Kibana.
