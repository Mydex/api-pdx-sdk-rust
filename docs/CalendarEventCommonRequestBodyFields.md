# CalendarEventCommonRequestBodyFields

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | Option<**String**> | Title of the event | [optional]
**description** | Option<**String**> | Detailed description of the event | [optional]
**start_timestamp** | Option<**i64**> | Start date and time as Unix timestamp | [optional]
**end_timestamp** | Option<**i64**> | End date and time as Unix timestamp | [optional]
**status** | Option<**Status**> | Status of the event (enum: INVITED, TENTATIVE, CONFIRMED, REJECTED, CANCELLED) | [optional][default to Tentative]
**organiser** | Option<**String**> | Creator of the event | [optional]
**attendee** | Option<**String**> | Person attending the event | [optional]
**location** | Option<**String**> | Event location | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


