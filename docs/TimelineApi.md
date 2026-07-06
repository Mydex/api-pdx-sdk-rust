# \TimelineApi

All URIs are relative to *https://api.mydex.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_timeline**](TimelineApi.md#get_timeline) | **GET** /timeline | Retrieve list of timeline items.
[**get_timeline_item**](TimelineApi.md#get_timeline_item) | **GET** /timeline/single-item | Retrieve a single timeline item.



## get_timeline

> models::TimelineResponse get_timeline(connection_token, uid, con_id)
Retrieve list of timeline items.

Returns a list of timeline items which includes: referrals, calendar events and secure messages.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |

### Return type

[**models::TimelineResponse**](TimelineResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_timeline_item

> models::TimelineSingleItemResponse get_timeline_item(connection_token, uid, con_id, feature_block, feature_block_id)
Retrieve a single timeline item.

Returns a single timeline item based on feature block and feature block id requested e.g. a 'referral' with id 123.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**feature_block** | **String** | The feature block the teimline item belongs to | [required] |
**feature_block_id** | **i32** | The specific ID of the record within the specified feature block e.g. if 'referrals' is the feature block, then this should be a specific referral id | [required] |

### Return type

[**models::TimelineSingleItemResponse**](TimelineSingleItemResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

