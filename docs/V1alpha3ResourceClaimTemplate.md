# V1alpha3ResourceClaimTemplate

ResourceClaimTemplate is used to produce ResourceClaim objects.  This is an alpha type and requires enabling the DynamicResourceAllocation feature gate.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | **str** | APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources | [optional] 
**kind** | **str** | Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds | [optional] 
**metadata** | [**V1ObjectMeta**](V1ObjectMeta.md) | Standard object metadata | [optional] 
**spec** | [**V1alpha3ResourceClaimTemplateSpec**](V1alpha3ResourceClaimTemplateSpec.md) | Describes the ResourceClaim that is to be generated.  This field is immutable. A ResourceClaim will get created by the control plane for a Pod when needed and then not get updated anymore. | 

## Example

```python
from kubernetes.models.v1alpha3_resource_claim_template import V1alpha3ResourceClaimTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of V1alpha3ResourceClaimTemplate from a JSON string
v1alpha3_resource_claim_template_instance = V1alpha3ResourceClaimTemplate.from_json(json)
# print the JSON string representation of the object
print(V1alpha3ResourceClaimTemplate.to_json())

# convert the object into a dict
v1alpha3_resource_claim_template_dict = v1alpha3_resource_claim_template_instance.to_dict()
# create an instance of V1alpha3ResourceClaimTemplate from a dict
v1alpha3_resource_claim_template_from_dict = V1alpha3ResourceClaimTemplate.from_dict(v1alpha3_resource_claim_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


