# SendSmsMessagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_text** | **str** |  | [optional] 
**message_encoding** | **str** |  | [optional] 
**data_coding** | **int** |  | [optional] 
**tpvp** | **int** |  | [optional] 
**callback_param** | [**SendSmsMessagesRequestCallbackParam**](SendSmsMessagesRequestCallbackParam.md) |  | [optional] 

## Example

```python
from jasperclient.models.send_sms_messages_request import SendSmsMessagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SendSmsMessagesRequest from a JSON string
send_sms_messages_request_instance = SendSmsMessagesRequest.from_json(json)
# print the JSON string representation of the object
print(SendSmsMessagesRequest.to_json())

# convert the object into a dict
send_sms_messages_request_dict = send_sms_messages_request_instance.to_dict()
# create an instance of SendSmsMessagesRequest from a dict
send_sms_messages_request_from_dict = SendSmsMessagesRequest.from_dict(send_sms_messages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


