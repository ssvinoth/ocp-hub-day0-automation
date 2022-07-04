# Required Vars :


```
# To be passed for every operator
operator_namespace: 'openshift-operators'
operator_name: 'elasticsearch-eck-operator-certified'
# This kustomize dirs are inside the roles/install_ocp_operator/kustomize dirs
kustomize_dir: 'gitops-catalog/elasticsearch-eck/operator/overlays/stable'


# Can be set as hostvars : localhost
ocp_api_url: https://api.cluster-dt7pv.dt7pv.sandbox1439.opentlc.com:6443
ocp_base_domain: cluster-dt7pv.dt7pv.sandbox1439.opentlc.com
oc_api_token: 'sha256~50wLzXtZAypkXfCBimmdM4gtjqyVa3jiY4RzBiWodaY'
oc_api_verify_ssl: false
 
```