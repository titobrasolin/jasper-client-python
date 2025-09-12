# DeviceDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**iccid** | **str** | ICCID del dispositivo. | [optional] 
**imsi** | **str** | IMSI del dispositivo. | [optional] 
**msisdn** | **str** | MSISDN o numero di telefono del dispositivo. | [optional] 
**imei** | **str** | IMEI del dispositivo. | [optional] 
**status** | **str** | Stato SIM del dispositivo. | [optional] 
**rate_plan** | **str** | Nome del piano tariffario associato al dispositivo. | [optional] 
**communication_plan** | **str** | Nome del piano di comunicazione associato al dispositivo. | [optional] 
**customer** | **str** | Nome del cliente (in genere un&#39;azienda o una business unit), eventualmente associato a questo dispositivo. | [optional] 
**end_consumer_id** | **str** | ID della persona eventualmente associata a questo dispositivo. | [optional] 
**date_activated** | **datetime** | Data di attivazione del dispositivo. | [optional] 
**date_added** | **datetime** | Data in cui il dispositivo è stato aggiunto. | [optional] 
**date_updated** | **datetime** | Data in cui si ha avuto luogo l&#39;ultimo aggiornamento delle informazioni relative al dispositivo. | [optional] 
**date_shipped** | **datetime** | Data in cui la SIM del dispositivo è stata trasferita dal magazzino del provider di servizi all&#39;Account aziendale. | [optional] 
**account_id** | **str** | ID dell&#39;account aziendale eventualmente associato al dispositivo. | [optional] 
**fixed_ip_address** | **str** | L&#39;indirizzo IPv4 assegnato al dispositivo. | [optional] 
**fixed_ipv6_address** | **str** | L&#39;indirizzo IPv6 assegnato al dispositivo. | [optional] 
**operator_custom1** | **str** | Valore per il campo personalizzato 1 del dispositivo creato dal provider di servizi. | [optional] 
**operator_custom2** | **str** | Valore per il campo personalizzato 2 del dispositivo creato dal provider di servizi. | [optional] 
**operator_custom3** | **str** | Valore per il campo personalizzato 3 del dispositivo creato dal provider di servizi. | [optional] 
**operator_custom4** | **str** | Valore per il campo personalizzato 4 del dispositivo creato dal provider di servizi. | [optional] 
**operator_custom5** | **str** | Valore per il campo personalizzato 5 del dispositivo creato dal provider di servizi. | [optional] 
**account_custom1** | **str** | Valore per il campo personalizzato 1 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom2** | **str** | Valore per il campo personalizzato 2 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom3** | **str** | Valore per il campo personalizzato 3 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom4** | **str** | Valore per il campo personalizzato 4 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom5** | **str** | Valore per il campo personalizzato 5 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom6** | **str** | Valore per il campo personalizzato 6 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom7** | **str** | Valore per il campo personalizzato 7 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom8** | **str** | Valore per il campo personalizzato 8 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom9** | **str** | Valore per il campo personalizzato 9 del dispositivo creato dall&#39;azienda. | [optional] 
**account_custom10** | **str** | Valore per il campo personalizzato 10 del dispositivo creato dall&#39;azienda. | [optional] 
**customer_custom1** | **str** | Valore per il campo personalizzato 1 del dispositivo creato dal cliente. | [optional] 
**customer_custom2** | **str** | Valore per il campo personalizzato 2 del dispositivo creato dal cliente. | [optional] 
**customer_custom3** | **str** | Valore per il campo personalizzato 3 del dispositivo creato dal cliente. | [optional] 
**customer_custom4** | **str** | Valore per il campo personalizzato 4 del dispositivo creato dal cliente. | [optional] 
**customer_custom5** | **str** | Valore per il campo personalizzato 5 del dispositivo creato dal cliente. | [optional] 
**sim_notes** | **str** | Informazioni che il provider di servizi ha aggiunto sul dispositivo. | [optional] 
**device_id** | **str** | Identificatore facoltativo che un account o un cliente può assegnare a un dispositivo. | [optional] 
**modem_id** | **str** | Identifica il modem utilizzato dal dispositivo per trasmettere dati. | [optional] 
**global_sim_type** | **str** | Indica se il dispositivo utilizza una SIM principale o una sottoscrizione virtuale di un partner (per funzionalità Global SIM). | [optional] 
**eid** | **str** | Identificatore eSIM che associa un profilo in Control Center con un&#39;eSIM. | [optional] 
**sim_profile_id** | **str** | Un identificativo che definisce il tipo di SIM fornito dal produttore. | [optional] 

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


