# Swagger\Client\GetQRCodeApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiSyncQrGetGet**](GetQRCodeApi.md#apisyncqrgetget) | **GET** /api/sync/qr/get | Получить QR код из WhatsApp для авторизации

# **apiSyncQrGetGet**
> \Swagger\Client\Model\InlineResponse2003 apiSyncQrGetGet($profile_id, $image_type)

Получить QR код из WhatsApp для авторизации

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GetQRCodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$image_type = "base64"; // string | В каком формате получить qr код

try {
    $result = $apiInstance->apiSyncQrGetGet($profile_id, $image_type);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GetQRCodeApi->apiSyncQrGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **image_type** | **string**| В каком формате получить qr код | [optional] [default to base64]

### Return type

[**\Swagger\Client\Model\InlineResponse2003**](../Model/InlineResponse2003.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

