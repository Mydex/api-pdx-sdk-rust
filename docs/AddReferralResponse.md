# AddReferralResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | Option<**i32**> | Indicates success | [optional]
**status** | Option<**Status**> | 'complete' when the member is already connected to the remote DSSA; 'pending' when the member needs to complete the FTC flow (enum: complete, pending) | [optional]
**message** | Option<**String**> | Present only when status is 'pending'. Describes the pending action taken. | [optional]
**url** | Option<**String**> | FTC URL the member should be redirected to. Present only when status is 'pending' and member_present is true. | [optional]
**qr** | Option<**String**> | QR code data URI for the FTC URL. Present only when status is 'pending' and member_present is true. | [optional]
**referral_id** | Option<**i32**> | ID of the newly created referral | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


