# Check if everything is ok
```
ansible nuage_k8s_master -i k8s-hosts -m ping
ansible nuage_k8s -i k8s-hosts -m ping -e cluter_name=nuage_k8s
```

# Run playbook
```
ansible-playbook -i k8s-hosts -e cluster_name=nuage_k8s nuage-cluster-1.5-create.yml
ansible-playbook -i k8s-hosts -e cluster_name=nuage_k8s nuage-4.0-k8s-plugin.yml
```

# Destroy cluster
```
ansible-playbook -i k8s-hosts -e cluster_name=nuage_k8s nuage-cluster-1.5-destroy.yml
```
