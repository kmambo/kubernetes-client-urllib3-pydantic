# V1Lifecycle

Lifecycle describes actions that the management system should take in response to container lifecycle events. For the PostStart and PreStop lifecycle handlers, management of the container blocks until the action is complete, unless the container process fails, in which case the handler is aborted.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**post_start** | [**V1LifecycleHandler**](V1LifecycleHandler.md) | PostStart is called immediately after a container is created. If the handler fails, the container is terminated and restarted according to its restart policy. Other management of the container blocks until the hook completes. More info: https://kubernetes.io/docs/concepts/containers/container-lifecycle-hooks/#container-hooks | [optional] 
**pre_stop** | [**V1LifecycleHandler**](V1LifecycleHandler.md) | PreStop is called immediately before a container is terminated due to an API request or management event such as liveness/startup probe failure, preemption, resource contention, etc. The handler is not called if the container crashes or exits. The Pod&#39;s termination grace period countdown begins before the PreStop hook is executed. Regardless of the outcome of the handler, the container will eventually terminate within the Pod&#39;s termination grace period (unless delayed by finalizers). Other management of the container blocks until the hook completes or until the termination grace period is reached. More info: https://kubernetes.io/docs/concepts/containers/container-lifecycle-hooks/#container-hooks | [optional] 

## Example

```python
from kubernetes.models.v1_lifecycle import V1Lifecycle

# TODO update the JSON string below
json = "{}"
# create an instance of V1Lifecycle from a JSON string
v1_lifecycle_instance = V1Lifecycle.from_json(json)
# print the JSON string representation of the object
print(V1Lifecycle.to_json())

# convert the object into a dict
v1_lifecycle_dict = v1_lifecycle_instance.to_dict()
# create an instance of V1Lifecycle from a dict
v1_lifecycle_from_dict = V1Lifecycle.from_dict(v1_lifecycle_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


