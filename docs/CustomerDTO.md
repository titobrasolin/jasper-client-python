# CustomerDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**security_question** | **str** |  | [optional] 
**security_answer** | **str** |  | [optional] 
**ship_to_bill_address** | **bool** |  | [optional] [default to False]
**contacts** | **List[object]** |  | [optional] 
**billing_address** | [**CustomerDTOBillingAddress**](CustomerDTOBillingAddress.md) |  | [optional] 
**shipping_address** | [**CustomerDTOBillingAddress**](CustomerDTOBillingAddress.md) |  | [optional] 

## Example

```python
from jasperclient.models.customer_dto import CustomerDTO

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerDTO from a JSON string
customer_dto_instance = CustomerDTO.from_json(json)
# print the JSON string representation of the object
print(CustomerDTO.to_json())

# convert the object into a dict
customer_dto_dict = customer_dto_instance.to_dict()
# create an instance of CustomerDTO from a dict
customer_dto_from_dict = CustomerDTO.from_dict(customer_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


