# DeviceEditModel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**effective_date** | **datetime** |  | [optional] 
**rate_plan** | **str** |  | [optional] 
**communication_plan** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**customer** | **str** |  | [optional] 
**device_id** | **str** |  | [optional] 
**modem_id** | **str** |  | [optional] 
**overage_limit_override** | **str** |  | [optional] 
**operator_custom1** | **str** |  | [optional] 
**operator_custom2** | **str** |  | [optional] 
**operator_custom3** | **str** |  | [optional] 
**operator_custom4** | **str** |  | [optional] 
**operator_custom5** | **str** |  | [optional] 
**account_custom1** | **str** |  | [optional] 
**account_custom2** | **str** |  | [optional] 
**account_custom3** | **str** |  | [optional] 
**account_custom4** | **str** |  | [optional] 
**account_custom5** | **str** |  | [optional] 
**account_custom6** | **str** |  | [optional] 
**account_custom7** | **str** |  | [optional] 
**account_custom8** | **str** |  | [optional] 
**account_custom9** | **str** |  | [optional] 
**account_custom10** | **str** |  | [optional] 
**customer_custom1** | **str** |  | [optional] 
**customer_custom2** | **str** |  | [optional] 
**customer_custom3** | **str** |  | [optional] 
**customer_custom4** | **str** |  | [optional] 
**customer_custom5** | **str** |  | [optional] 
**ipv4_address** | **str** |  | [optional] 
**ipv6_address** | **str** |  | [optional] 

## Example

```python
from jasperclient.models.device_edit_model import DeviceEditModel

# TODO update the JSON string below
json = "{}"
# create an instance of DeviceEditModel from a JSON string
device_edit_model_instance = DeviceEditModel.from_json(json)
# print the JSON string representation of the object
print(DeviceEditModel.to_json())

# convert the object into a dict
device_edit_model_dict = device_edit_model_instance.to_dict()
# create an instance of DeviceEditModel from a dict
device_edit_model_from_dict = DeviceEditModel.from_dict(device_edit_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


