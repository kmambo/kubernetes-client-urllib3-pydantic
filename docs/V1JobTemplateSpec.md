# V1JobTemplateSpec

JobTemplateSpec describes the data a Job should have when created from a template

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**V1ObjectMeta**](V1ObjectMeta.md) | Standard object&#39;s metadata of the jobs created from this template. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata | [optional] 
**spec** | [**V1JobSpec**](V1JobSpec.md) | Specification of the desired behavior of the job. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status | [optional] 

## Example

```python
from kubernetes.models.v1_job_template_spec import V1JobTemplateSpec

# TODO update the JSON string below
json = "{}"
# create an instance of V1JobTemplateSpec from a JSON string
v1_job_template_spec_instance = V1JobTemplateSpec.from_json(json)
# print the JSON string representation of the object
print(V1JobTemplateSpec.to_json())

# convert the object into a dict
v1_job_template_spec_dict = v1_job_template_spec_instance.to_dict()
# create an instance of V1JobTemplateSpec from a dict
v1_job_template_spec_from_dict = V1JobTemplateSpec.from_dict(v1_job_template_spec_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


