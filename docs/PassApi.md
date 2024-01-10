# IO.Swagger.Api.PassApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateOrUpdatePass**](PassApi.md#createorupdatepass) | **POST** /pass | This method creates or (if the pass id already exists) updates a pass, so you don&#39;t have to track ids and creation status of your passes.
[**DeletePass**](PassApi.md#deletepass) | **DELETE** /pass | Delete pass by pass id.
[**GetPass**](PassApi.md#getpass) | **GET** /pass | Get pass information by pass id.
[**PassList**](PassApi.md#passlist) | **GET** /pass/list | Retrieve the list of active pass ids for a given pass type.
[**PassSync**](PassApi.md#passsync) | **POST** /pass/sync | Send updates to all active passes for a given pass type.


<a name="createorupdatepass"></a>
# **CreateOrUpdatePass**
> void CreateOrUpdatePass (Object passTypeId, Object passId = null)

This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateOrUpdatePassExample
    {
        public void main()
        {
            var apiInstance = new PassApi();
            var passTypeId = new Object(); // Object | your pass type id, for example P963493 (Urban Fitness)
            var passId = new Object(); // Object | id of the pass (provided by you when creating the pass or automatically set by passmeister) (optional) 

            try
            {
                // This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.
                apiInstance.CreateOrUpdatePass(passTypeId, passId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PassApi.CreateOrUpdatePass: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](Object.md)| your pass type id, for example P963493 (Urban Fitness) | 
 **passId** | [**Object**](Object.md)| id of the pass (provided by you when creating the pass or automatically set by passmeister) | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="deletepass"></a>
# **DeletePass**
> void DeletePass (Object passTypeId, Object passId)

Delete pass by pass id.

Delete pass by pass id.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class DeletePassExample
    {
        public void main()
        {
            var apiInstance = new PassApi();
            var passTypeId = new Object(); // Object | your pass type id, for example P963493 (Urban Fitness)
            var passId = new Object(); // Object | id of the pass

            try
            {
                // Delete pass by pass id.
                apiInstance.DeletePass(passTypeId, passId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PassApi.DeletePass: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](Object.md)| your pass type id, for example P963493 (Urban Fitness) | 
 **passId** | [**Object**](Object.md)| id of the pass | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="getpass"></a>
# **GetPass**
> void GetPass (Object passTypeId, Object passId)

Get pass information by pass id.

Get pass information by pass id.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetPassExample
    {
        public void main()
        {
            var apiInstance = new PassApi();
            var passTypeId = new Object(); // Object | your pass type id, for example P963493 (Urban Fitness)
            var passId = new Object(); // Object | id of the pass

            try
            {
                // Get pass information by pass id.
                apiInstance.GetPass(passTypeId, passId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PassApi.GetPass: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](Object.md)| your pass type id, for example P963493 (Urban Fitness) | 
 **passId** | [**Object**](Object.md)| id of the pass | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="passlist"></a>
# **PassList**
> void PassList (Object passTypeId, Object page = null, Object limit = null)

Retrieve the list of active pass ids for a given pass type.

Retrieve the list of active pass ids for a given pass type.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class PassListExample
    {
        public void main()
        {
            var apiInstance = new PassApi();
            var passTypeId = new Object(); // Object | your pass type id, for example P963493 (Urban Fitness)
            var page = new Object(); // Object |  (optional) 
            var limit = new Object(); // Object |  (optional) 

            try
            {
                // Retrieve the list of active pass ids for a given pass type.
                apiInstance.PassList(passTypeId, page, limit);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PassApi.PassList: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](Object.md)| your pass type id, for example P963493 (Urban Fitness) | 
 **page** | [**Object**](Object.md)|  | [optional] 
 **limit** | [**Object**](Object.md)|  | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="passsync"></a>
# **PassSync**
> void PassSync (Object passTypeId)

Send updates to all active passes for a given pass type.

For example: you changed the pass type layout and now you want to update all installed passes. (The API call only confirms the scheduling of the updates, actual updating of passes on your customers devices can take a while.)

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class PassSyncExample
    {
        public void main()
        {
            var apiInstance = new PassApi();
            var passTypeId = new Object(); // Object | your pass type id, for example P963493 (Urban Fitness)

            try
            {
                // Send updates to all active passes for a given pass type.
                apiInstance.PassSync(passTypeId);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PassApi.PassSync: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**Object**](Object.md)| your pass type id, for example P963493 (Urban Fitness) | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

