# DeviceDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**iccid** | **str** | The ICCID of the device. | [optional] 
**imsi** | **str** | The device IMSI. | [optional] 
**msisdn** | **str** | The device MSISDN or phone number. | [optional] 
**imei** | **str** | The device IMEI. | [optional] 
**status** | **str** | The device SIM status. | [optional] 
**rate_plan** | **str** | The name of the rate plan associated with the device. | [optional] 
**communication_plan** | **str** | The name of the communication plan associated with the device. | [optional] 
**customer** | **str** | The name of the customer (generally an enterprise or business unit), if any, associated with this device. | [optional] 
**end_consumer_id** | **str** | The ID of the person, if any, associated with this device. | [optional] 
**date_activated** | **datetime** | The date when the device was first activated. | [optional] 
**date_added** | **datetime** | The date when the device was added. | [optional] 
**date_updated** | **datetime** | The date when the last device information update occurred. | [optional] 
**date_shipped** | **datetime** | The date when the device SIM was transferred from the operator inventory into the enterprise account. | [optional] 
**account_id** | **str** | The ID of the enterprise account associated with the device. | [optional] 
**fixed_ip_address** | **str** | The IPv4 address assigned to the device. This field may be null if the device communication plan uses dynamic IP addresses or if the device uses an IPv6 address instead. | [optional] 
**fixed_ipv6_address** | **str** | The IPv6 address assigned to the device. This field may be null if the device communication plan uses dynamic IP addresses or if the device uses an IPv4 address instead. | [optional] 
**operator_custom1** | **str** | Value for custom device field 1 created by the operator. | [optional] 
**operator_custom2** | **str** | Value for custom device field 2 created by the operator. | [optional] 
**operator_custom3** | **str** | Value for custom device field 3 created by the operator. | [optional] 
**operator_custom4** | **str** | Value for custom device field 4 created by the operator. | [optional] 
**operator_custom5** | **str** | Value for custom device field 5 created by the operator. | [optional] 
**account_custom1** | **str** | Value for custom device field 1 created by the enterprise. | [optional] 
**account_custom2** | **str** | Value for custom device field 2 created by the enterprise. | [optional] 
**account_custom3** | **str** | Value for custom device field 3 created by the enterprise. | [optional] 
**account_custom4** | **str** | Value for custom device field 4 created by the enterprise. | [optional] 
**account_custom5** | **str** | Value for custom device field 5 created by the enterprise. | [optional] 
**account_custom6** | **str** | Value for custom device field 6 created by the enterprise. | [optional] 
**account_custom7** | **str** | Value for custom device field 7 created by the enterprise. | [optional] 
**account_custom8** | **str** | Value for custom device field 8 created by the enterprise. | [optional] 
**account_custom9** | **str** | Value for custom device field 9 created by the enterprise. | [optional] 
**account_custom10** | **str** | Value for custom device field 10 created by the enterprise. | [optional] 
**customer_custom1** | **str** | Value for custom device field 1 created by the customer. | [optional] 
**customer_custom2** | **str** | Value for custom device field 2 created by the customer. | [optional] 
**customer_custom3** | **str** | Value for custom device field 3 created by the customer. | [optional] 
**customer_custom4** | **str** | Value for custom device field 4 created by the customer. | [optional] 
**customer_custom5** | **str** | Value for custom device field 5 created by the customer. | [optional] 
**sim_notes** | **str** | Information the operator has added about the device. | [optional] 
**device_id** | **str** | Optional identifier that an account or customer can give to a device. | [optional] 
**modem_id** | **str** | Identifies the modem used by the device to transmit data. | [optional] 
**global_sim_type** | **str** | For enterprises taking advantage of Control Center&#39;s Global SIM feature, this value indicates whether the device is using a primary SIM from the lead operator or a virtual subscription from a partner operator. | [optional] 
**eid** | **str** | An eSIM identifier that associates a profile in Control Center with an eSIM. | [optional] 
**sim_profile_id** | **str** | An identifier that defines the type of SIM provided by the manufacturer. | [optional] 
**example** | **object** |  | [optional] 

## Example

```python
from jasperclient.models.device_details import DeviceDetails

# TODO update the JSON string below
json = "{}"
# create an instance of DeviceDetails from a JSON string
device_details_instance = DeviceDetails.from_json(json)
# print the JSON string representation of the object
print(DeviceDetails.to_json())

# convert the object into a dict
device_details_dict = device_details_instance.to_dict()
# create an instance of DeviceDetails from a dict
device_details_from_dict = DeviceDetails.from_dict(device_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


