# CustomerDTOBillingAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_line1** | **str** |  | [optional] 
**address_line2** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**country** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 

## Example

```python
from jasperclient.models.customer_dto_billing_address import CustomerDTOBillingAddress

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerDTOBillingAddress from a JSON string
customer_dto_billing_address_instance = CustomerDTOBillingAddress.from_json(json)
# print the JSON string representation of the object
print(CustomerDTOBillingAddress.to_json())

# convert the object into a dict
customer_dto_billing_address_dict = customer_dto_billing_address_instance.to_dict()
# create an instance of CustomerDTOBillingAddress from a dict
customer_dto_billing_address_from_dict = CustomerDTOBillingAddress.from_dict(customer_dto_billing_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


