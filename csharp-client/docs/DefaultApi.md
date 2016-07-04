# IO.Swagger.Api.DefaultApi

All URIs are relative to *https://api.pbxdom.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CallsGet**](DefaultApi.md#callsget) | **GET** /Calls | 
[**FeaturesChartsGet**](DefaultApi.md#featureschartsget) | **GET** /Features/charts | 
[**FeaturesReportsGet**](DefaultApi.md#featuresreportsget) | **GET** /Features/reports | 
[**FeaturesWidgetGet**](DefaultApi.md#featureswidgetget) | **GET** /Features/widget | 


# **CallsGet**
> List<InlineResponse200> CallsGet (double? rptType, double? rptId, decimal? start = null, decimal? limit = null, string sortBy = null, string sortType = null, string fromDate = null, string toDate = null, decimal? duration = null, string phone = null, string phone1 = null, string co = null, string ext = null, decimal? pbxId = null, decimal? callSource = null, decimal? callType = null, decimal? direction = null, string callerName = null, string did = null, string dnis = null, string acc = null, decimal? ring = null, decimal? cost = null, decimal? group = null)



Gets `Calls` info. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CallsGetExample
    {
        public void main()
        {
            
            var apiInstance = new DefaultApi();
            var rptType = 1.2;  // double? | Report type. (0 report, 1 widget, 2 chart).
            var rptId = 1.2;  // double? | Report id.
            var start = 3.4;  // decimal? | Start offset. (optional) 
            var limit = 3.4;  // decimal? | Number of results to return. Max 10K. (optional) 
            var sortBy = sortBy_example;  // string | Sort column. (optional) 
            var sortType = sortType_example;  // string | Sort mode asc/desc. (optional) 
            var fromDate = fromDate_example;  // string | Start date time. (optional) 
            var toDate = toDate_example;  // string | End date time. (optional) 
            var duration = 3.4;  // decimal? | Duration range. (optional) 
            var phone = phone_example;  // string | List of caller phone. (optional) 
            var phone1 = phone1_example;  // string | List of dialled phones. (optional) 
            var co = co_example;  // string | List of trunk/co. (optional) 
            var ext = ext_example;  // string | list of extensions. (optional) 
            var pbxId = 3.4;  // decimal? | list of PBX Ids. (optional) 
            var callSource = 3.4;  // decimal? | list of callsource. (optional) 
            var callType = 3.4;  // decimal? | list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls) (optional) 
            var direction = 3.4;  // decimal? | list of direction.(0 incoming, 1 outgoing, 2 internal) (optional) 
            var callerName = callerName_example;  // string | list of caller name. (optional) 
            var did = did_example;  // string | list of did. (optional) 
            var dnis = dnis_example;  // string | list of dnis. (optional) 
            var acc = acc_example;  // string | list of account code. (optional) 
            var ring = 3.4;  // decimal? | Ring range.Seconds unit. (optional) 
            var cost = 3.4;  // decimal? | Cost range. (optional) 
            var group = 3.4;  // decimal? | Department/Group id. (optional) 

            try
            {
                List&lt;InlineResponse200&gt; result = apiInstance.CallsGet(rptType, rptId, start, limit, sortBy, sortType, fromDate, toDate, duration, phone, phone1, co, ext, pbxId, callSource, callType, direction, callerName, did, dnis, acc, ring, cost, group);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling DefaultApi.CallsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rptType** | **double?**| Report type. (0 report, 1 widget, 2 chart). | 
 **rptId** | **double?**| Report id. | 
 **start** | **decimal?**| Start offset. | [optional] 
 **limit** | **decimal?**| Number of results to return. Max 10K. | [optional] 
 **sortBy** | **string**| Sort column. | [optional] 
 **sortType** | **string**| Sort mode asc/desc. | [optional] 
 **fromDate** | **string**| Start date time. | [optional] 
 **toDate** | **string**| End date time. | [optional] 
 **duration** | **decimal?**| Duration range. | [optional] 
 **phone** | **string**| List of caller phone. | [optional] 
 **phone1** | **string**| List of dialled phones. | [optional] 
 **co** | **string**| List of trunk/co. | [optional] 
 **ext** | **string**| list of extensions. | [optional] 
 **pbxId** | **decimal?**| list of PBX Ids. | [optional] 
 **callSource** | **decimal?**| list of callsource. | [optional] 
 **callType** | **decimal?**| list of call type signatures.(5 Unanswered Calls, 7 Transfered Calls, 8 Forwarded Calls) | [optional] 
 **direction** | **decimal?**| list of direction.(0 incoming, 1 outgoing, 2 internal) | [optional] 
 **callerName** | **string**| list of caller name. | [optional] 
 **did** | **string**| list of did. | [optional] 
 **dnis** | **string**| list of dnis. | [optional] 
 **acc** | **string**| list of account code. | [optional] 
 **ring** | **decimal?**| Ring range.Seconds unit. | [optional] 
 **cost** | **decimal?**| Cost range. | [optional] 
 **group** | **decimal?**| Department/Group id. | [optional] 

### Return type

[**List<InlineResponse200>**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FeaturesChartsGet**
> List<InlineResponse200> FeaturesChartsGet ()



Gets `Charts` list. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FeaturesChartsGetExample
    {
        public void main()
        {
            
            var apiInstance = new DefaultApi();

            try
            {
                List&lt;InlineResponse200&gt; result = apiInstance.FeaturesChartsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling DefaultApi.FeaturesChartsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List<InlineResponse200>**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FeaturesReportsGet**
> List<InlineResponse200> FeaturesReportsGet ()



Gets `Reports` list. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FeaturesReportsGetExample
    {
        public void main()
        {
            
            var apiInstance = new DefaultApi();

            try
            {
                List&lt;InlineResponse200&gt; result = apiInstance.FeaturesReportsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling DefaultApi.FeaturesReportsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List<InlineResponse200>**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FeaturesWidgetGet**
> List<InlineResponse200> FeaturesWidgetGet ()



Gets `Widgets` list. 

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class FeaturesWidgetGetExample
    {
        public void main()
        {
            
            var apiInstance = new DefaultApi();

            try
            {
                List&lt;InlineResponse200&gt; result = apiInstance.FeaturesWidgetGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling DefaultApi.FeaturesWidgetGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List<InlineResponse200>**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

