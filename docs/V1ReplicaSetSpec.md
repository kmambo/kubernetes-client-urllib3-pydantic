# V1ReplicaSetSpec

ReplicaSetSpec is the specification of a ReplicaSet.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**min_ready_seconds** | **int** | Minimum number of seconds for which a newly created pod should be ready without any of its container crashing, for it to be considered available. Defaults to 0 (pod will be considered available as soon as it is ready) | [optional] 
**replicas** | **int** | Replicas is the number of desired replicas. This is a pointer to distinguish between explicit zero and unspecified. Defaults to 1. More info: https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller/#what-is-a-replicationcontroller | [optional] 
**selector** | [**V1LabelSelector**](V1LabelSelector.md) | Selector is a label query over pods that should match the replica count. Label keys and values that must match in order to be controlled by this replica set. It must match the pod template&#39;s labels. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors | 
**template** | [**V1PodTemplateSpec**](V1PodTemplateSpec.md) | Template is the object that describes the pod that will be created if insufficient replicas are detected. More info: https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller#pod-template | [optional] 

## Example

```python
from kubernetes.models.v1_replica_set_spec import V1ReplicaSetSpec

# TODO update the JSON string below
json = "{}"
# create an instance of V1ReplicaSetSpec from a JSON string
v1_replica_set_spec_instance = V1ReplicaSetSpec.from_json(json)
# print the JSON string representation of the object
print(V1ReplicaSetSpec.to_json())

# convert the object into a dict
v1_replica_set_spec_dict = v1_replica_set_spec_instance.to_dict()
# create an instance of V1ReplicaSetSpec from a dict
v1_replica_set_spec_from_dict = V1ReplicaSetSpec.from_dict(v1_replica_set_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


