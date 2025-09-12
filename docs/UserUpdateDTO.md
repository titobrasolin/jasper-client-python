# UserUpdateDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role_name** | **str** |  | [optional] 
**access_type** | **str** |  | [optional] 
**user_locked** | **bool** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**language** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 
**live_update_enabled** | **bool** |  | [optional] 

## Example

```python
from jasperclient.models.user_update_dto import UserUpdateDTO

# TODO update the JSON string below
json = "{}"
# create an instance of UserUpdateDTO from a JSON string
user_update_dto_instance = UserUpdateDTO.from_json(json)
# print the JSON string representation of the object
print(UserUpdateDTO.to_json())

# convert the object into a dict
user_update_dto_dict = user_update_dto_instance.to_dict()
# create an instance of UserUpdateDTO from a dict
user_update_dto_from_dict = UserUpdateDTO.from_dict(user_update_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


