# CalendarAppointmentCreateRequestBody

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
**context** | **Context** | The context the appointment belongs to e.g. a referral (enum: referral) | 
**context_id** | **i32** | The id of the specific context record that this appointment relates to e.g. the referral id | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


