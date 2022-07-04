# ocp-hub-day0-automation

# Requires following collections : 
- kubernetes.core 
- community.general
- ansible.builtin
- community.okd (Not used)

# Requires OCP connection details
Set the vars in the host_vars/localhost/

# Day 0 operations on hub cluster 

## Install following operators
1. gitops operator
2. rh sso operator
3. acm operator
4. acs operator
5. eck operator
6. cluster logging operator

## Install the instances and configure 
1. gitops operator
    - no config
2. rh sso operator
    - install sso (keycloak) instance
    -  [MANUAL] configure instance and connect to ocp !! (for now MANUAL)    
3. acm operator
    - install acm instance : MultiClusterHub
    - no config required
4. acs operator
    - install central instance
    -  [MANUAL] install securecluster (MANUAL)
5. eck operator
    - install elastic search instance
    - install kibana instance
6. cluster logging operator
    - install clusterlogging instance
    - install clusterloggingforwarder instance



