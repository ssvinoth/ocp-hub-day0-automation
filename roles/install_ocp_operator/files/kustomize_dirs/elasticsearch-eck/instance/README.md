# ECK Elasticsearch and Kibana Instances

Installs a elastic search and kibana instance.

`elasticsearch` base directory will install a `7.12.0` version of elasticsearch in `elastic-monitoring` namespace with `100gi` PVC. The name of the instance will be `elasticsearch`. 

`kibana` base directory will install a `7.12.0` version of kibana in `elastic-monitoring` namespace. It will get associated with the elasticsearch instance with the name `elasticsearch`. 

PLEASE use *overlays* directory to customize your instances. Eg., change pvc size, name etc.,

## Usage

If you have cloned the `gitops-catalog` repository, you can install the elasticsearch and kibana instances based on the choice of base or overlay (custom) directory.

```
oc apply -k elasticsearch-eck/instance/elasticsearch/base
oc apply -k elasticsearch-eck/instance/kibana/base
```
