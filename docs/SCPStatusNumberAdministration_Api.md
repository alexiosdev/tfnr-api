# TfnrApIs.SCPStatusNumberAdministration_Api

All URIs are relative to *https://api-devp-tfnregistry.somos.com/v1/ip*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sCPStatusNumberDeletebyRequestId**](SCPStatusNumberAdministration_Api.md#sCPStatusNumberDeletebyRequestId) | **GET** /scp/delete/number/{requestId} | SCP Status Number Delete - Sync Timeout 
[**scpStatusNumberAudit**](SCPStatusNumberAdministration_Api.md#scpStatusNumberAudit) | **PUT** /scp/audit/number | SCP Status Number Audit 
[**scpStatusNumberAuditbyRequestId**](SCPStatusNumberAdministration_Api.md#scpStatusNumberAuditbyRequestId) | **GET** /scp/audit/number/{requestId} | SCP Status Number Audit - Sync Timeout 
[**scpStatusNumberDelete**](SCPStatusNumberAdministration_Api.md#scpStatusNumberDelete) | **PUT** /scp/delete/number | SCP Status Number Delete 
[**scpStatusNumberQuery**](SCPStatusNumberAdministration_Api.md#scpStatusNumberQuery) | **GET** /scp/query/number | SCP Status Query 
[**scpStatusNumberQuerybyRequestId**](SCPStatusNumberAdministration_Api.md#scpStatusNumberQuerybyRequestId) | **GET** /scp/query/number/{requestId} | SCP Status Number Query - Sync Timeout 
[**scpStatusNumberResend**](SCPStatusNumberAdministration_Api.md#scpStatusNumberResend) | **PUT** /scp/resend/number | SCP Resend 
[**scpStatusNumberResendbyRequestId**](SCPStatusNumberAdministration_Api.md#scpStatusNumberResendbyRequestId) | **GET** /scp/resend/number/{requestId} | SCP Resend - Sync Timeout 


<a name="sCPStatusNumberDeletebyRequestId"></a>
# **sCPStatusNumberDeletebyRequestId**
> DeleteNumberResponse sCPStatusNumberDeletebyRequestId(authorization, requestId)

SCP Status Number Delete - Sync Timeout 

This API is used to delete a customer record (CR), or pointer record from given SCPs. The status of a record for an SCP is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message.

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let requestId = 789; // Number | RequestId returned due to timeout


apiInstance.sCPStatusNumberDeletebyRequestId(authorization, requestId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **requestId** | **Number**| RequestId returned due to timeout | 

### Return type

[**DeleteNumberResponse**](DeleteNumberResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="scpStatusNumberAudit"></a>
# **scpStatusNumberAudit**
> AuditStatusNumberResponse scpStatusNumberAudit(authorization, body)

SCP Status Number Audit 

This API is used to audit the status of a customer record (CR), or pointer record at given SCPs by number. The status of a record for an SCP is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message.

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let body = new TfnrApIs.AuditStatusNumberRequest(); // AuditStatusNumberRequest | 


apiInstance.scpStatusNumberAudit(authorization, body, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **body** | [**AuditStatusNumberRequest**](AuditStatusNumberRequest.md)|  | 

### Return type

[**AuditStatusNumberResponse**](AuditStatusNumberResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="scpStatusNumberAuditbyRequestId"></a>
# **scpStatusNumberAuditbyRequestId**
> AuditStatusNumberResponse scpStatusNumberAuditbyRequestId(authorization, requestId)

SCP Status Number Audit - Sync Timeout 

This API is used to audit the status of a customer record (CR, or pointer record at given SCPs by number. The status of a record for an SCP is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message.

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let requestId = 789; // Number | RequestId returned due to timeout


apiInstance.scpStatusNumberAuditbyRequestId(authorization, requestId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **requestId** | **Number**| RequestId returned due to timeout | 

### Return type

[**AuditStatusNumberResponse**](AuditStatusNumberResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="scpStatusNumberDelete"></a>
# **scpStatusNumberDelete**
> DeleteNumberResponse scpStatusNumberDelete(authorization, body)

SCP Status Number Delete 

This API is used to delete a customer record (CR), or pointer record from given SCPs. The status of a record for an SCP is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message. 

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let body = new TfnrApIs.DeleteNumberRequest(); // DeleteNumberRequest | 


apiInstance.scpStatusNumberDelete(authorization, body, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **body** | [**DeleteNumberRequest**](DeleteNumberRequest.md)|  | 

### Return type

[**DeleteNumberResponse**](DeleteNumberResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="scpStatusNumberQuery"></a>
# **scpStatusNumberQuery**
> SCPQueryNumberResponse scpStatusNumberQuery(authorization, recNum, opts)

SCP Status Query 

This API is used to query the status of SCP(s) for one customer record (CR), or pointer record by number. The status of a record for an SCP is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message. 

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let recNum = "recNum_example"; // String | The Dialed Telephone Number identifying the record.

let opts = { 
  'effDtTm': "effDtTm_example" // String | Effective date and time of the record 
};

apiInstance.scpStatusNumberQuery(authorization, recNum, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **recNum** | **String**| The Dialed Telephone Number identifying the record. | 
 **effDtTm** | **String**| Effective date and time of the record  | [optional] 

### Return type

[**SCPQueryNumberResponse**](SCPQueryNumberResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="scpStatusNumberQuerybyRequestId"></a>
# **scpStatusNumberQuerybyRequestId**
> SCPQueryNumberResponse scpStatusNumberQuerybyRequestId(authorization, requestId)

SCP Status Number Query - Sync Timeout 

This API is used to retrieve the status of a record for an SCP. This is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message. 

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let requestId = 789; // Number | RequestId returned due to timeout


apiInstance.scpStatusNumberQuerybyRequestId(authorization, requestId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **requestId** | **Number**| RequestId returned due to timeout | 

### Return type

[**SCPQueryNumberResponse**](SCPQueryNumberResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="scpStatusNumberResend"></a>
# **scpStatusNumberResend**
> SCPResendResponse scpStatusNumberResend(authorization, body)

SCP Resend 

This API is used to resend a Customer, or Pointer record to given SCPs. The status of a record for an SCP is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message. 

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let body = new TfnrApIs.SCPResendRequest(); // SCPResendRequest | 


apiInstance.scpStatusNumberResend(authorization, body, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **body** | [**SCPResendRequest**](SCPResendRequest.md)|  | 

### Return type

[**SCPResendResponse**](SCPResendResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="scpStatusNumberResendbyRequestId"></a>
# **scpStatusNumberResendbyRequestId**
> SCPResendResponse scpStatusNumberResendbyRequestId(authorization, requestId)

SCP Resend - Sync Timeout 

This API is used to resend a Customer, or Pointer record to given SCPs. The status of a record for an SCP is reflected by one of several possible status values that are automatically generated by IP or returned by the SCP. The SCP status values for the requested record are shown in the response message.

### Example
```javascript
import TfnrApIs from 'tfnr_ap_is';

let apiInstance = new TfnrApIs.SCPStatusNumberAdministration_Api();

let authorization = "authorization_example"; // String | Bearer access_token

let requestId = 789; // Number | RequestId returned due to timeout


apiInstance.scpStatusNumberResendbyRequestId(authorization, requestId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **String**| Bearer access_token | 
 **requestId** | **Number**| RequestId returned due to timeout | 

### Return type

[**SCPResendResponse**](SCPResendResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json
