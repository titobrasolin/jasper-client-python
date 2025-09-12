# EditEventInstancesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_id** | **str** |  | [optional] [default to '123456']
**event_name** | **str** |  | [optional] [default to 'eventName']
**action** | **str** |  | [default to 'CancelPendingEvents']

## Example

```python
from jasperclient.models.edit_event_instances_request import EditEventInstancesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditEventInstancesRequest from a JSON string
edit_event_instances_request_instance = EditEventInstancesRequest.from_json(json)
# print the JSON string representation of the object
print(EditEventInstancesRequest.to_json())

# convert the object into a dict
edit_event_instances_request_dict = edit_event_instances_request_instance.to_dict()
# create an instance of EditEventInstancesRequest from a dict
edit_event_instances_request_from_dict = EditEventInstancesRequest.from_dict(edit_event_instances_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


