# \ReferralsApi

All URIs are relative to *https://api.mydex.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_all_referrals**](ReferralsApi.md#get_all_referrals) | **GET** /referrals/read-all | Retrieve rall referrals for a given member.
[**get_single_referral**](ReferralsApi.md#get_single_referral) | **GET** /referrals/read-single | Retrieve a single referral by id for a given member.
[**post_self_referral**](ReferralsApi.md#post_self_referral) | **POST** /referrals/self-refer | Supports self-referral.
[**update_referral_status**](ReferralsApi.md#update_referral_status) | **PUT** /referrals/update-status | Supports updating the status of a referral.



## get_all_referrals

> models::ReferralListResponse get_all_referrals(connection_token, uid, con_id)
Retrieve rall referrals for a given member.

Returns a list of referrals.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |

### Return type

[**models::ReferralListResponse**](ReferralListResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_single_referral

> models::ReferralSingleResponse get_single_referral(connection_token, uid, con_id, id)
Retrieve a single referral by id for a given member.

Returns the requested referral.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**id** | **String** | The record id requested. | [required] |

### Return type

[**models::ReferralSingleResponse**](ReferralSingleResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## post_self_referral

> models::CreateResponse post_self_referral(connection_token, uid, con_id, self_referral_request_body)
Supports self-referral.

Creates a new referral of type 'Self Referred' in the member's PDS.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**self_referral_request_body** | Option<[**SelfReferralRequestBody**](SelfReferralRequestBody.md)> |  |  |

### Return type

[**models::CreateResponse**](CreateResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_referral_status

> models::UpdateResponse update_referral_status(connection_token, uid, con_id, referral_status_update_request_body)
Supports updating the status of a referral.

Updates the status of a member's referral specified by id. For example, having been referred to a service, the status is set by default to 'Referred' and this route enables it to be updated to 'Accepted' or 'Rejected'

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**connection_token** | **String** | Member's Connection Key | [required] |
**uid** | **String** | The unique ID of a mydex member | [required] |
**con_id** | **String** | The connection_id is a shared id between a connection and a member. It is a hyphenated combination of the member UID and the Dedicated Connection NID. | [required] |
**referral_status_update_request_body** | Option<[**ReferralStatusUpdateRequestBody**](ReferralStatusUpdateRequestBody.md)> |  |  |

### Return type

[**models::UpdateResponse**](UpdateResponse.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

