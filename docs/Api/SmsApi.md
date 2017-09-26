# NotifyLk\SmsApi

All URIs are relative to *https://app.notify.lk/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sendSMS**](SmsApi.md#sendSMS) | **POST** /send | Sending SMS to a number from specified sender ID


# **sendSMS**
> sendSMS($userId, $apiKey, $message, $to, $senderId, $contact_fname, $contact_lname, $contact_email, $contact_address)

Sending SMS to a number from specified sender ID

Sends SMS to any number

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new NotifyLk\Api\SmsApi();
$userId = "userId_example"; // string | API User ID - Can be found in your settings page.
$apiKey = "apiKey_example"; // string | API Secret - Can be found in your settings page.
$message = "message_example"; // string | Text of the message. 320 chars max.
$to = "to_example"; // string | Number to send the SMS. Better to use 9471XXXXXXX format.
$senderId = "senderId_example"; // string | This is the from name recipient will see as the sender of the SMS. Use \"NotifyDemo\" if you have not ordered your own sender ID yet.
$contact_fname = "contact_fname_example"; // string | Contact First Name - This will be used while saving the phone number in your Notify contacts.
$contact_lname = "contact_lname_example"; // string | Contact Last Name - This will be used while saving the phone number in your Notify contacts.
$contact_email = "contact_email_example"; // string | Contact Email Address - This will be used while saving the phone number in your Notify contacts.
$contact_address = "contact_address_example"; // string | Contact Physical Address - This will be used while saving the phone number in your Notify contacts.

try {
    $api_instance->sendSMS($userId, $apiKey, $message, $to, $senderId, $contact_fname, $contact_lname, $contact_email, $contact_address);
} catch (Exception $e) {
    echo 'Exception when calling SmsApi->sendSMS: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **string**| API User ID - Can be found in your settings page. |
 **apiKey** | **string**| API Secret - Can be found in your settings page. |
 **message** | **string**| Text of the message. 320 chars max. |
 **to** | **string**| Number to send the SMS. Better to use 9471XXXXXXX format. |
 **senderId** | **string**| This is the from name recipient will see as the sender of the SMS. Use \&quot;NotifyDemo\&quot; if you have not ordered your own sender ID yet. |
 **contact_fname** | **string**| Contact First Name - This will be used while saving the phone number in your Notify contacts. | [optional]
 **contact_lname** | **string**| Contact Last Name - This will be used while saving the phone number in your Notify contacts. | [optional]
 **contact_email** | **string**| Contact Email Address - This will be used while saving the phone number in your Notify contacts. | [optional]
 **contact_address** | **string**| Contact Physical Address - This will be used while saving the phone number in your Notify contacts. | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/application/x-www-form-urlencoded

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)
