# CalendarEventCreateRequestBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **String** | Title of the event | 
**description** | Option<**String**> | Detailed description of the event | [optional]
**start_timestamp** | **i64** | Start date and time as Unix timestamp | 
**end_timestamp** | **i64** | End date and time as Unix timestamp | 
**status** | **Status** | Status of the event (enum: INVITED, TENTATIVE, CONFIRMED, REJECTED, CANCELLED) | [default to Tentative]
**organiser** | Option<**String**> | Creator of the event | [optional]
**attendee** | Option<**String**> | Person attending the event | [optional]
**location** | Option<**String**> | Event location | [optional]
**r#type** | Option<**Type**> | Type of event (enum: Appointment) | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


