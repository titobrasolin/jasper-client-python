# ActivateTerminalEventRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_name** | **str** |  | [default to 'eventName']
**effective_date** | **datetime** |  | [optional] 
**instances** | **int** |  | [optional] [default to 1]
**unlimited_instances** | **bool** |  | [optional] [default to False]

## Example

```python
from jasperclient.models.activate_terminal_event_request import ActivateTerminalEventRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ActivateTerminalEventRequest from a JSON string
activate_terminal_event_request_instance = ActivateTerminalEventRequest.from_json(json)
# print the JSON string representation of the object
print(ActivateTerminalEventRequest.to_json())

# convert the object into a dict
activate_terminal_event_request_dict = activate_terminal_event_request_instance.to_dict()
# create an instance of ActivateTerminalEventRequest from a dict
activate_terminal_event_request_from_dict = ActivateTerminalEventRequest.from_dict(activate_terminal_event_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


