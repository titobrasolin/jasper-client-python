# UserCreateDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | [optional] 
**role_name** | **str** |  | [optional] 
**access_type** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**customer_name** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**language** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 
**live_update_enabled** | **bool** |  | [optional] 

## Example

```python
from jasperclient.models.user_create_dto import UserCreateDTO

# TODO update the JSON string below
json = "{}"
# create an instance of UserCreateDTO from a JSON string
user_create_dto_instance = UserCreateDTO.from_json(json)
# print the JSON string representation of the object
print(UserCreateDTO.to_json())

# convert the object into a dict
user_create_dto_dict = user_create_dto_instance.to_dict()
# create an instance of UserCreateDTO from a dict
user_create_dto_from_dict = UserCreateDTO.from_dict(user_create_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


