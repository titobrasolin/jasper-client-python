# Hello


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | **str** |  | [optional] 

## Example

```python
from jasperclient.models.hello import Hello

# TODO update the JSON string below
json = "{}"
# create an instance of Hello from a JSON string
hello_instance = Hello.from_json(json)
# print the JSON string representation of the object
print(Hello.to_json())

# convert the object into a dict
hello_dict = hello_instance.to_dict()
# create an instance of Hello from a dict
hello_from_dict = Hello.from_dict(hello_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


