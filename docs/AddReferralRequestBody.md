# AddReferralRequestBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**remote_dssa_uuid** | **uuid::Uuid** | UUIDv4 of the remote DSSA the referral is being made to | 
**member_present** | **bool** | Whether the member is present to complete the FTC flow. If true, an FTC URL is returned for immediate redirect. If false, a notification is sent to the member. | 
**return_to** | **String** | URL the member is redirected to after completing the FTC flow | 
**referral_data** | [**models::AddReferralData**](AddReferralData.md) |  | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


