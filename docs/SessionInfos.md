# SessionInfos


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**iccid** | **str** |  | [optional] 
**ip_address** | **str** |  | [optional] 
**ipv6_address** | **str** |  | [optional] 
**date_session_started** | **datetime** |  | [optional] 
**date_session_ended** | **datetime** |  | [optional] 
**apn** | **str** |  | [optional] 

## Example

```python
from jasperclient.models.session_infos import SessionInfos

# TODO update the JSON string below
json = "{}"
# create an instance of SessionInfos from a JSON string
session_infos_instance = SessionInfos.from_json(json)
# print the JSON string representation of the object
print(SessionInfos.to_json())

# convert the object into a dict
session_infos_dict = session_infos_instance.to_dict()
# create an instance of SessionInfos from a dict
session_infos_from_dict = SessionInfos.from_dict(session_infos_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


