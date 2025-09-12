# SendSmsMessagesRequestCallbackParam


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**callback_type** | **str** |  | [optional] 
**callback_url** | **str** |  | [optional] 

## Example

```python
from jasperclient.models.send_sms_messages_request_callback_param import SendSmsMessagesRequestCallbackParam

# TODO update the JSON string below
json = "{}"
# create an instance of SendSmsMessagesRequestCallbackParam from a JSON string
send_sms_messages_request_callback_param_instance = SendSmsMessagesRequestCallbackParam.from_json(json)
# print the JSON string representation of the object
print(SendSmsMessagesRequestCallbackParam.to_json())

# convert the object into a dict
send_sms_messages_request_callback_param_dict = send_sms_messages_request_callback_param_instance.to_dict()
# create an instance of SendSmsMessagesRequestCallbackParam from a dict
send_sms_messages_request_callback_param_from_dict = SendSmsMessagesRequestCallbackParam.from_dict(send_sms_messages_request_callback_param_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


