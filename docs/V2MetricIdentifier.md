# V2MetricIdentifier

MetricIdentifier defines the name and optionally selector for a metric

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | name is the name of the given metric | [default to '']
**selector** | [**V1LabelSelector**](V1LabelSelector.md) | selector is the string-encoded form of a standard kubernetes label selector for the given metric When set, it is passed as an additional parameter to the metrics server for more specific metrics scoping. When unset, just the metricName will be used to gather metrics. | [optional] 

## Example

```python
from kubernetes.models.v2_metric_identifier import V2MetricIdentifier

# TODO update the JSON string below
json = "{}"
# create an instance of V2MetricIdentifier from a JSON string
v2_metric_identifier_instance = V2MetricIdentifier.from_json(json)
# print the JSON string representation of the object
print(V2MetricIdentifier.to_json())

# convert the object into a dict
v2_metric_identifier_dict = v2_metric_identifier_instance.to_dict()
# create an instance of V2MetricIdentifier from a dict
v2_metric_identifier_from_dict = V2MetricIdentifier.from_dict(v2_metric_identifier_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


