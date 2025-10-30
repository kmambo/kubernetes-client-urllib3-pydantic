# V1DaemonSet

DaemonSet represents the configuration of a daemon set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** | APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources | [optional] 
**kind** | **str** | Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds | [optional] 
**metadata** | [**V1ObjectMeta**](V1ObjectMeta.md) | Standard object&#39;s metadata. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata | [optional] 
**spec** | [**V1DaemonSetSpec**](V1DaemonSetSpec.md) | The desired behavior of this daemon set. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status | [optional] 
**status** | [**V1DaemonSetStatus**](V1DaemonSetStatus.md) | The current status of this daemon set. This data may be out of date by some window of time. Populated by the system. Read-only. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status | [optional] 

## Example

```python
from kubernetes.models.v1_daemon_set import V1DaemonSet

# TODO update the JSON string below
json = "{}"
# create an instance of V1DaemonSet from a JSON string
v1_daemon_set_instance = V1DaemonSet.from_json(json)
# print the JSON string representation of the object
print(V1DaemonSet.to_json())

# convert the object into a dict
v1_daemon_set_dict = v1_daemon_set_instance.to_dict()
# create an instance of V1DaemonSet from a dict
v1_daemon_set_from_dict = V1DaemonSet.from_dict(v1_daemon_set_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


