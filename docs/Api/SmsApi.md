# NotifyLk\SmsApi

All URIs are relative to *https://app.notify.lk/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sendSMS**](SmsApi.md#sendSMS) | **POST** /send | Sending SMS to a number from specified sender ID


# **sendSMS**
> sendSMS($user_id, $api_key, $message, $to, $sender_id, $contact_fname, $contact_lname, $contact_email, $contact_address, $contact_group)

Sending SMS to a number from specified sender ID

Sends SMS to any number

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new NotifyLk\Api\SmsApi();
$user_id = "user_id_example"; // string | API User ID - Can be found in your settings page.
$api_key = "api_key_example"; // string | API Key - Can be found in your settings page.
$message = "message_example"; // string | Text of the message. 320 chars max.
$to = "to_example"; // string | Number to send the SMS. Better to use 9471XXXXXXX format.
$sender_id = "sender_id_example"; // string | This is the from name recipient will see as the sender of the SMS. Use \\\"NotifyDemo\\\" if you have not ordered your own sender ID yet.
$contact_fname = "contact_fname_example"; // string | Contact First Name - This will be used while saving the phone number in your Notify contacts.
$contact_lname = "contact_lname_example"; // string | Contact Last Name - This will be used while saving the phone number in your Notify contacts.
$contact_email = "example@domain.com"; // string | Contact Email Address - This will be used while saving the phone number in your Notify contacts.
$contact_address = "contact_address_example"; // string | Contact Physical Address - This will be used while saving the phone number in your Notify contacts.
$contact_group = 0; // int | A group ID to associate the saving contact with

try {
    $api_instance->sendSMS($user_id, $api_key, $message, $to, $sender_id, $contact_fname, $contact_lname, $contact_email, $contact_address, $contact_group);
} catch (Exception $e) {
    echo 'Exception when calling SmsApi->sendSMS: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **string**| API User ID - Can be found in your settings page. |
 **api_key** | **string**| API Key - Can be found in your settings page. |
 **message** | **string**| Text of the message. 320 chars max. |
 **to** | **string**| Number to send the SMS. Better to use 9471XXXXXXX format. |
 **sender_id** | **string**| This is the from name recipient will see as the sender of the SMS. Use \\\&quot;NotifyDemo\\\&quot; if you have not ordered your own sender ID yet. |
 **contact_fname** | **string**| Contact First Name - This will be used while saving the phone number in your Notify contacts. | [optional]
 **contact_lname** | **string**| Contact Last Name - This will be used while saving the phone number in your Notify contacts. | [optional]
 **contact_email** | **string**| Contact Email Address - This will be used while saving the phone number in your Notify contacts. | [optional]
 **contact_address** | **string**| Contact Physical Address - This will be used while saving the phone number in your Notify contacts. | [optional]
 **contact_group** | **int**| A group ID to associate the saving contact with | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/application/x-www-form-urlencoded

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

