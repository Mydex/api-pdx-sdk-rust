# \CalendarApi

All URIs are relative to *https://api.mydex.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_calendar_event**](CalendarApi.md#delete_calendar_event) | **DELETE** /calendar/delete-event | Supports deleting a calendar-event.
[**get_calendar_appointments**](CalendarApi.md#get_calendar_appointments) | **GET** /calendar/get-appointments | Retrieve appointments for a given context
[**get_calendar_events**](CalendarApi.md#get_calendar_events) | **GET** /calendar/get-events | Retrieve calendar events
[**post_calendar_appointment**](CalendarApi.md#post_calendar_appointment) | **POST** /calendar/add-appointment | Supports adding a calendar-appointment.
[**post_calendar_event**](CalendarApi.md#post_calendar_event) | **POST** /calendar/add-event | Supports adding a calendar-event.
[**put_calendar_event**](CalendarApi.md#put_calendar_event) | **PUT** /calendar/update-event | Supports updating a calendar-event.



## delete_calendar_event

> models::DeleteResponse delete_calendar_event(connection_token, uid, con_id, calendar_event_delete_request_body)
Supports deleting a calendar-event.

Deletes an event in the user's calendar.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**calendar_event_delete_request_body** | Option<[**CalendarEventDeleteRequestBody**](CalendarEventDeleteRequestBody.md)> |  |  |

### Return type

[**models::DeleteResponse**](DeleteResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_calendar_appointments

> models::GetAppointmentsResponse get_calendar_appointments(connection_token, uid, con_id, context, context_id)
Retrieve appointments for a given context

Returns a list of appointments filtered by context and context_id.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**context** | **String** | The context this belongs to | [required] |
**context_id** | **i32** | The specific ID of the context record | [required] |

### Return type

[**models::GetAppointmentsResponse**](GetAppointmentsResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_calendar_events

> models::GetEventsResponse get_calendar_events(connection_token, uid, con_id)
Retrieve calendar events

Returns a list of calendar events.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |

### Return type

[**models::GetEventsResponse**](GetEventsResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_calendar_appointment

> models::CreateResponse post_calendar_appointment(connection_token, uid, con_id, calendar_appointment_create_request_body)
Supports adding a calendar-appointment.

Creates a new appointment in the user's calendar. An appointment must be made within a specified context e.g. a 'Referral'

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**calendar_appointment_create_request_body** | Option<[**CalendarAppointmentCreateRequestBody**](CalendarAppointmentCreateRequestBody.md)> |  |  |

### Return type

[**models::CreateResponse**](CreateResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_calendar_event

> models::CreateResponse post_calendar_event(connection_token, uid, con_id, calendar_event_create_request_body)
Supports adding a calendar-event.

Creates a new event in the user's calendar.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**calendar_event_create_request_body** | Option<[**CalendarEventCreateRequestBody**](CalendarEventCreateRequestBody.md)> |  |  |

### Return type

[**models::CreateResponse**](CreateResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## put_calendar_event

> models::UpdateResponse put_calendar_event(connection_token, uid, con_id, calendar_event_update_request_body)
Supports updating a calendar-event.

Updates an event in the user's calendar. For example, updating the 'status' from 'INVITED' to 'CONFIRMED' when a user accepts the invitation to an appointment.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**calendar_event_update_request_body** | Option<[**CalendarEventUpdateRequestBody**](CalendarEventUpdateRequestBody.md)> |  |  |

### Return type

[**models::UpdateResponse**](UpdateResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

