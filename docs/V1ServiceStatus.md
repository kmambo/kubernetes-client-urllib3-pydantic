# V1ServiceStatus

ServiceStatus represents the current status of a service.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conditions** | [**List[V1Condition]**](V1Condition.md) | Current service state | [optional] 
**load_balancer** | [**V1LoadBalancerStatus**](V1LoadBalancerStatus.md) | LoadBalancer contains the current status of the load-balancer, if one is present. | [optional] 

## Example

```python
from kubernetes.models.v1_service_status import V1ServiceStatus

# TODO update the JSON string below
json = "{}"
# create an instance of V1ServiceStatus from a JSON string
v1_service_status_instance = V1ServiceStatus.from_json(json)
# print the JSON string representation of the object
print(V1ServiceStatus.to_json())

# convert the object into a dict
v1_service_status_dict = v1_service_status_instance.to_dict()
# create an instance of V1ServiceStatus from a dict
v1_service_status_from_dict = V1ServiceStatus.from_dict(v1_service_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


