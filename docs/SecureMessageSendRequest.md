# SecureMessageSendRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **String** | Content of the message | 
**conversation_id** | **String** | ID of the conversation formatted like {context}-{context_id} where context is e.g. 'referral' and context_id is the id of the specifc record in that context. | 
**service_identifier** | Option<**uuid::Uuid**> | A UUIDv4 that uniquely identifies the service this message relates to. Optional, but when present allows the SP to link the message to a specific service. | [optional]
**service_id** | Option<**i32**> | ID of the service this message relates to. Optional. | [optional]
**message_to** | **String** | Recipient user ID | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


