# \SecureMessagesApi

All URIs are relative to *https://api.mydex.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_secure_message_conversation**](SecureMessagesApi.md#get_secure_message_conversation) | **GET** /secure-messages/conversation | Retrieve all secure messages for a given conversation.
[**post_secure_message_receive**](SecureMessagesApi.md#post_secure_message_receive) | **POST** /secure-messages/receive | Supports sending a message to the member's PDS.
[**post_secure_message_send**](SecureMessagesApi.md#post_secure_message_send) | **POST** /secure-messages/send | Supports sending a message from the member's PDS.



## get_secure_message_conversation

> models::SecureMessageConversationResponse get_secure_message_conversation(connection_token, uid, con_id, conversation_id)
Retrieve all secure messages for a given conversation.

Returns a list of secure messages that form part of a conversation.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**conversation_id** | **String** | The specific ID of the conversation that groups messages together | [required] |

### Return type

[**models::SecureMessageConversationResponse**](SecureMessageConversationResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_secure_message_receive

> models::CreateResponse post_secure_message_receive(connection_token, uid, con_id, secure_message_receive_request)
Supports sending a message to the member's PDS.

Creates a new received message in the member's PDS.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**secure_message_receive_request** | Option<[**SecureMessageReceiveRequest**](SecureMessageReceiveRequest.md)> |  |  |

### Return type

[**models::CreateResponse**](CreateResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_secure_message_send

> models::CreateResponse post_secure_message_send(connection_token, uid, con_id, secure_message_send_request)
Supports sending a message from the member's PDS.

Creates a new sent message in the member's PDS.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**secure_message_send_request** | Option<[**SecureMessageSendRequest**](SecureMessageSendRequest.md)> |  |  |

### Return type

[**models::CreateResponse**](CreateResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

