# Swagger\Client\DefaultApi

All URIs are relative to *https://www.sendowl.com/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createBundle**](DefaultApi.md#createbundle) | **POST** /packages | Create a new bundle
[**deleteBundle**](DefaultApi.md#deletebundle) | **DELETE** /packages/{package_id} | Delete a bundle
[**deleteOrder**](DefaultApi.md#deleteorder) | **DELETE** /orders/{order_id} | Delete an order
[**getBundle**](DefaultApi.md#getbundle) | **GET** /packages/{package_id} | Get a specific bundle
[**getBundles**](DefaultApi.md#getbundles) | **GET** /packages | List all bundles
[**getOrder**](DefaultApi.md#getorder) | **GET** /orders/{order_id} | Get a specific order
[**getOrders**](DefaultApi.md#getorders) | **GET** /orders | List all orders
[**refundOrder**](DefaultApi.md#refundorder) | **POST** /orders/{order_id}/refund | Refund an order
[**resendOrderEmail**](DefaultApi.md#resendorderemail) | **POST** /orders/{order_id}/resend_email | Resend order emails
[**searchOrders**](DefaultApi.md#searchorders) | **GET** /orders/search | Search orders
[**updateBundle**](DefaultApi.md#updatebundle) | **PUT** /packages/{package_id} | Update a bundle
[**updateOrder**](DefaultApi.md#updateorder) | **PUT** /orders/{order_id} | Update an order

# **createBundle**
> \Swagger\Client\Model\Bundle createBundle($body)

Create a new bundle

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Bundle(); // \Swagger\Client\Model\Bundle | 

try {
    $result = $apiInstance->createBundle($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createBundle: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Bundle**](../Model/Bundle.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\Bundle**](../Model/Bundle.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteBundle**
> deleteBundle($package_id)

Delete a bundle

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$package_id = 56; // int | 

try {
    $apiInstance->deleteBundle($package_id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteBundle: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **package_id** | **int**|  |

### Return type

void (empty response body)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteOrder**
> deleteOrder($order_id)

Delete an order

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_id = 56; // int | 

try {
    $apiInstance->deleteOrder($order_id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteOrder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **int**|  |

### Return type

void (empty response body)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getBundle**
> \Swagger\Client\Model\Bundle getBundle($package_id)

Get a specific bundle

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$package_id = 56; // int | 

try {
    $result = $apiInstance->getBundle($package_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getBundle: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **package_id** | **int**|  |

### Return type

[**\Swagger\Client\Model\Bundle**](../Model/Bundle.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getBundles**
> \Swagger\Client\Model\Bundle[] getBundles()

List all bundles

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getBundles();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getBundles: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Bundle[]**](../Model/Bundle.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getOrder**
> \Swagger\Client\Model\Order getOrder($order_id)

Get a specific order

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_id = 56; // int | 

try {
    $result = $apiInstance->getOrder($order_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getOrder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **int**|  |

### Return type

[**\Swagger\Client\Model\Order**](../Model/Order.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getOrders**
> \Swagger\Client\Model\Order[] getOrders($from, $to, $orderable, $state, $referred_by, $sort)

List all orders

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$from = new \DateTime("2013-10-20"); // \DateTime | Start date for filtering orders
$to = new \DateTime("2013-10-20"); // \DateTime | End date for filtering orders
$orderable = "orderable_example"; // string | Filter orders by product, bundle or subscription
$state = "state_example"; // string | Filter orders by state
$referred_by = 56; // int | Filter orders by affiliate
$sort = "sort_example"; // string | Sort orders by newest first

try {
    $result = $apiInstance->getOrders($from, $to, $orderable, $state, $referred_by, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getOrders: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from** | **\DateTime**| Start date for filtering orders | [optional]
 **to** | **\DateTime**| End date for filtering orders | [optional]
 **orderable** | **string**| Filter orders by product, bundle or subscription | [optional]
 **state** | **string**| Filter orders by state | [optional]
 **referred_by** | **int**| Filter orders by affiliate | [optional]
 **sort** | **string**| Sort orders by newest first | [optional]

### Return type

[**\Swagger\Client\Model\Order[]**](../Model/Order.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **refundOrder**
> refundOrder($order_id, $body)

Refund an order

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_id = 56; // int | 
$body = new \Swagger\Client\Model\OrderIdRefundBody(); // \Swagger\Client\Model\OrderIdRefundBody | 

try {
    $apiInstance->refundOrder($order_id, $body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->refundOrder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **int**|  |
 **body** | [**\Swagger\Client\Model\OrderIdRefundBody**](../Model/OrderIdRefundBody.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **resendOrderEmail**
> resendOrderEmail($order_id, $body)

Resend order emails

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_id = 56; // int | 
$body = new \Swagger\Client\Model\OrderIdResendEmailBody(); // \Swagger\Client\Model\OrderIdResendEmailBody | 

try {
    $apiInstance->resendOrderEmail($order_id, $body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->resendOrderEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **int**|  |
 **body** | [**\Swagger\Client\Model\OrderIdResendEmailBody**](../Model/OrderIdResendEmailBody.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchOrders**
> \Swagger\Client\Model\Order[] searchOrders($term)

Search orders

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$term = "term_example"; // string | Search term (buyer email, buyer name, giftee email, giftee name, business name or transaction id)

try {
    $result = $apiInstance->searchOrders($term);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->searchOrders: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **term** | **string**| Search term (buyer email, buyer name, giftee email, giftee name, business name or transaction id) |

### Return type

[**\Swagger\Client\Model\Order[]**](../Model/Order.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateBundle**
> updateBundle($package_id, $body)

Update a bundle

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$package_id = 56; // int | 
$body = new \Swagger\Client\Model\Bundle(); // \Swagger\Client\Model\Bundle | 

try {
    $apiInstance->updateBundle($package_id, $body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->updateBundle: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **package_id** | **int**|  |
 **body** | [**\Swagger\Client\Model\Bundle**](../Model/Bundle.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateOrder**
> updateOrder($order_id, $body)

Update an order

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_id = 56; // int | 
$body = new \Swagger\Client\Model\Order(); // \Swagger\Client\Model\Order | 

try {
    $apiInstance->updateOrder($order_id, $body);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->updateOrder: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **int**|  |
 **body** | [**\Swagger\Client\Model\Order**](../Model/Order.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

