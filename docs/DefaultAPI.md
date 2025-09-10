# DefaultAPI

All URIs are relative to *https://api.optioffice.local/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orgsOrgIdDocumentsDocumentIdDelete**](DefaultAPI.md#orgsorgiddocumentsdocumentiddelete) | **DELETE** /orgs/{orgId}/documents/{documentId} | Delete document
[**orgsOrgIdDocumentsDocumentIdGet**](DefaultAPI.md#orgsorgiddocumentsdocumentidget) | **GET** /orgs/{orgId}/documents/{documentId} | Get document
[**orgsOrgIdDocumentsDocumentIdPut**](DefaultAPI.md#orgsorgiddocumentsdocumentidput) | **PUT** /orgs/{orgId}/documents/{documentId} | Update document
[**orgsOrgIdDocumentsGet**](DefaultAPI.md#orgsorgiddocumentsget) | **GET** /orgs/{orgId}/documents | List documents
[**orgsOrgIdDocumentsPost**](DefaultAPI.md#orgsorgiddocumentspost) | **POST** /orgs/{orgId}/documents | Upload document
[**orgsOrgIdLeadsGet**](DefaultAPI.md#orgsorgidleadsget) | **GET** /orgs/{orgId}/leads | List leads
[**orgsOrgIdLeadsLeadIdDelete**](DefaultAPI.md#orgsorgidleadsleadiddelete) | **DELETE** /orgs/{orgId}/leads/{leadId} | Delete lead
[**orgsOrgIdLeadsLeadIdGet**](DefaultAPI.md#orgsorgidleadsleadidget) | **GET** /orgs/{orgId}/leads/{leadId} | Get lead
[**orgsOrgIdLeadsLeadIdPut**](DefaultAPI.md#orgsorgidleadsleadidput) | **PUT** /orgs/{orgId}/leads/{leadId} | Update lead
[**orgsOrgIdLeadsPost**](DefaultAPI.md#orgsorgidleadspost) | **POST** /orgs/{orgId}/leads | Create lead
[**orgsOrgIdListingsGet**](DefaultAPI.md#orgsorgidlistingsget) | **GET** /orgs/{orgId}/listings | List listings
[**orgsOrgIdListingsListingIdDelete**](DefaultAPI.md#orgsorgidlistingslistingiddelete) | **DELETE** /orgs/{orgId}/listings/{listingId} | Delete listing
[**orgsOrgIdListingsListingIdGet**](DefaultAPI.md#orgsorgidlistingslistingidget) | **GET** /orgs/{orgId}/listings/{listingId} | Get listing
[**orgsOrgIdListingsListingIdPut**](DefaultAPI.md#orgsorgidlistingslistingidput) | **PUT** /orgs/{orgId}/listings/{listingId} | Update listing
[**orgsOrgIdListingsPost**](DefaultAPI.md#orgsorgidlistingspost) | **POST** /orgs/{orgId}/listings | Create listing
[**orgsOrgIdOfficesGet**](DefaultAPI.md#orgsorgidofficesget) | **GET** /orgs/{orgId}/offices | List offices
[**orgsOrgIdOfficesOfficeIdDelete**](DefaultAPI.md#orgsorgidofficesofficeiddelete) | **DELETE** /orgs/{orgId}/offices/{officeId} | Delete office
[**orgsOrgIdOfficesOfficeIdGet**](DefaultAPI.md#orgsorgidofficesofficeidget) | **GET** /orgs/{orgId}/offices/{officeId} | Get office
[**orgsOrgIdOfficesOfficeIdPut**](DefaultAPI.md#orgsorgidofficesofficeidput) | **PUT** /orgs/{orgId}/offices/{officeId} | Update office
[**orgsOrgIdOfficesPost**](DefaultAPI.md#orgsorgidofficespost) | **POST** /orgs/{orgId}/offices | Create office
[**orgsOrgIdPaymentsGet**](DefaultAPI.md#orgsorgidpaymentsget) | **GET** /orgs/{orgId}/payments | List payments
[**orgsOrgIdPaymentsPaymentIdDelete**](DefaultAPI.md#orgsorgidpaymentspaymentiddelete) | **DELETE** /orgs/{orgId}/payments/{paymentId} | Delete payment
[**orgsOrgIdPaymentsPaymentIdGet**](DefaultAPI.md#orgsorgidpaymentspaymentidget) | **GET** /orgs/{orgId}/payments/{paymentId} | Get payment
[**orgsOrgIdPaymentsPaymentIdPut**](DefaultAPI.md#orgsorgidpaymentspaymentidput) | **PUT** /orgs/{orgId}/payments/{paymentId} | Update payment
[**orgsOrgIdPaymentsPost**](DefaultAPI.md#orgsorgidpaymentspost) | **POST** /orgs/{orgId}/payments | Create payment


# **orgsOrgIdDocumentsDocumentIdDelete**
```swift
    open class func orgsOrgIdDocumentsDocumentIdDelete(orgId: String, documentId: String, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Delete document

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let documentId = "documentId_example" // String | 

// Delete document
DefaultAPI.orgsOrgIdDocumentsDocumentIdDelete(orgId: orgId, documentId: documentId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **documentId** | **String** |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdDocumentsDocumentIdGet**
```swift
    open class func orgsOrgIdDocumentsDocumentIdGet(orgId: String, documentId: String, completion: @escaping (_ data: Document?, _ error: Error?) -> Void)
```

Get document

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let documentId = "documentId_example" // String | 

// Get document
DefaultAPI.orgsOrgIdDocumentsDocumentIdGet(orgId: orgId, documentId: documentId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **documentId** | **String** |  | 

### Return type

[**Document**](Document.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdDocumentsDocumentIdPut**
```swift
    open class func orgsOrgIdDocumentsDocumentIdPut(orgId: String, documentId: String, document: Document, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Update document

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let documentId = "documentId_example" // String | 
let document = Document(id: "id_example", organizationId: "organizationId_example", name: "name_example", url: "url_example") // Document | 

// Update document
DefaultAPI.orgsOrgIdDocumentsDocumentIdPut(orgId: orgId, documentId: documentId, document: document) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **documentId** | **String** |  | 
 **document** | [**Document**](Document.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdDocumentsGet**
```swift
    open class func orgsOrgIdDocumentsGet(orgId: String, completion: @escaping (_ data: [Document]?, _ error: Error?) -> Void)
```

List documents

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 

// List documents
DefaultAPI.orgsOrgIdDocumentsGet(orgId: orgId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 

### Return type

[**[Document]**](Document.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdDocumentsPost**
```swift
    open class func orgsOrgIdDocumentsPost(orgId: String, document: Document, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Upload document

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let document = Document(id: "id_example", organizationId: "organizationId_example", name: "name_example", url: "url_example") // Document | 

// Upload document
DefaultAPI.orgsOrgIdDocumentsPost(orgId: orgId, document: document) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **document** | [**Document**](Document.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdLeadsGet**
```swift
    open class func orgsOrgIdLeadsGet(orgId: String, completion: @escaping (_ data: [Lead]?, _ error: Error?) -> Void)
```

List leads

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 

// List leads
DefaultAPI.orgsOrgIdLeadsGet(orgId: orgId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 

### Return type

[**[Lead]**](Lead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdLeadsLeadIdDelete**
```swift
    open class func orgsOrgIdLeadsLeadIdDelete(orgId: String, leadId: String, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Delete lead

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let leadId = "leadId_example" // String | 

// Delete lead
DefaultAPI.orgsOrgIdLeadsLeadIdDelete(orgId: orgId, leadId: leadId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **leadId** | **String** |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdLeadsLeadIdGet**
```swift
    open class func orgsOrgIdLeadsLeadIdGet(orgId: String, leadId: String, completion: @escaping (_ data: Lead?, _ error: Error?) -> Void)
```

Get lead

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let leadId = "leadId_example" // String | 

// Get lead
DefaultAPI.orgsOrgIdLeadsLeadIdGet(orgId: orgId, leadId: leadId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **leadId** | **String** |  | 

### Return type

[**Lead**](Lead.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdLeadsLeadIdPut**
```swift
    open class func orgsOrgIdLeadsLeadIdPut(orgId: String, leadId: String, lead: Lead, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Update lead

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let leadId = "leadId_example" // String | 
let lead = Lead(id: "id_example", contactId: "contactId_example", channel: "channel_example", status: "status_example") // Lead | 

// Update lead
DefaultAPI.orgsOrgIdLeadsLeadIdPut(orgId: orgId, leadId: leadId, lead: lead) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **leadId** | **String** |  | 
 **lead** | [**Lead**](Lead.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdLeadsPost**
```swift
    open class func orgsOrgIdLeadsPost(orgId: String, lead: Lead, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Create lead

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let lead = Lead(id: "id_example", contactId: "contactId_example", channel: "channel_example", status: "status_example") // Lead | 

// Create lead
DefaultAPI.orgsOrgIdLeadsPost(orgId: orgId, lead: lead) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **lead** | [**Lead**](Lead.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdListingsGet**
```swift
    open class func orgsOrgIdListingsGet(orgId: String, completion: @escaping (_ data: [Listing]?, _ error: Error?) -> Void)
```

List listings

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 

// List listings
DefaultAPI.orgsOrgIdListingsGet(orgId: orgId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 

### Return type

[**[Listing]**](Listing.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdListingsListingIdDelete**
```swift
    open class func orgsOrgIdListingsListingIdDelete(orgId: String, listingId: String, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Delete listing

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let listingId = "listingId_example" // String | 

// Delete listing
DefaultAPI.orgsOrgIdListingsListingIdDelete(orgId: orgId, listingId: listingId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **listingId** | **String** |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdListingsListingIdGet**
```swift
    open class func orgsOrgIdListingsListingIdGet(orgId: String, listingId: String, completion: @escaping (_ data: Listing?, _ error: Error?) -> Void)
```

Get listing

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let listingId = "listingId_example" // String | 

// Get listing
DefaultAPI.orgsOrgIdListingsListingIdGet(orgId: orgId, listingId: listingId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **listingId** | **String** |  | 

### Return type

[**Listing**](Listing.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdListingsListingIdPut**
```swift
    open class func orgsOrgIdListingsListingIdPut(orgId: String, listingId: String, listing: Listing, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Update listing

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let listingId = "listingId_example" // String | 
let listing = Listing(id: "id_example", officeId: "officeId_example", price: 123, status: "status_example") // Listing | 

// Update listing
DefaultAPI.orgsOrgIdListingsListingIdPut(orgId: orgId, listingId: listingId, listing: listing) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **listingId** | **String** |  | 
 **listing** | [**Listing**](Listing.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdListingsPost**
```swift
    open class func orgsOrgIdListingsPost(orgId: String, listing: Listing, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Create listing

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let listing = Listing(id: "id_example", officeId: "officeId_example", price: 123, status: "status_example") // Listing | 

// Create listing
DefaultAPI.orgsOrgIdListingsPost(orgId: orgId, listing: listing) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **listing** | [**Listing**](Listing.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdOfficesGet**
```swift
    open class func orgsOrgIdOfficesGet(orgId: String, completion: @escaping (_ data: [Office]?, _ error: Error?) -> Void)
```

List offices

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 

// List offices
DefaultAPI.orgsOrgIdOfficesGet(orgId: orgId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 

### Return type

[**[Office]**](Office.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdOfficesOfficeIdDelete**
```swift
    open class func orgsOrgIdOfficesOfficeIdDelete(orgId: String, officeId: String, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Delete office

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let officeId = "officeId_example" // String | 

// Delete office
DefaultAPI.orgsOrgIdOfficesOfficeIdDelete(orgId: orgId, officeId: officeId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **officeId** | **String** |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdOfficesOfficeIdGet**
```swift
    open class func orgsOrgIdOfficesOfficeIdGet(orgId: String, officeId: String, completion: @escaping (_ data: Office?, _ error: Error?) -> Void)
```

Get office

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let officeId = "officeId_example" // String | 

// Get office
DefaultAPI.orgsOrgIdOfficesOfficeIdGet(orgId: orgId, officeId: officeId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **officeId** | **String** |  | 

### Return type

[**Office**](Office.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdOfficesOfficeIdPut**
```swift
    open class func orgsOrgIdOfficesOfficeIdPut(orgId: String, officeId: String, office: Office, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Update office

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let officeId = "officeId_example" // String | 
let office = Office(id: "id_example", organizationId: "organizationId_example", title: "title_example", description: "description_example") // Office | 

// Update office
DefaultAPI.orgsOrgIdOfficesOfficeIdPut(orgId: orgId, officeId: officeId, office: office) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **officeId** | **String** |  | 
 **office** | [**Office**](Office.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdOfficesPost**
```swift
    open class func orgsOrgIdOfficesPost(orgId: String, office: Office, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Create office

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let office = Office(id: "id_example", organizationId: "organizationId_example", title: "title_example", description: "description_example") // Office | 

// Create office
DefaultAPI.orgsOrgIdOfficesPost(orgId: orgId, office: office) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **office** | [**Office**](Office.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdPaymentsGet**
```swift
    open class func orgsOrgIdPaymentsGet(orgId: String, completion: @escaping (_ data: [Payment]?, _ error: Error?) -> Void)
```

List payments

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 

// List payments
DefaultAPI.orgsOrgIdPaymentsGet(orgId: orgId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 

### Return type

[**[Payment]**](Payment.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdPaymentsPaymentIdDelete**
```swift
    open class func orgsOrgIdPaymentsPaymentIdDelete(orgId: String, paymentId: String, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Delete payment

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let paymentId = "paymentId_example" // String | 

// Delete payment
DefaultAPI.orgsOrgIdPaymentsPaymentIdDelete(orgId: orgId, paymentId: paymentId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **paymentId** | **String** |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdPaymentsPaymentIdGet**
```swift
    open class func orgsOrgIdPaymentsPaymentIdGet(orgId: String, paymentId: String, completion: @escaping (_ data: Payment?, _ error: Error?) -> Void)
```

Get payment

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let paymentId = "paymentId_example" // String | 

// Get payment
DefaultAPI.orgsOrgIdPaymentsPaymentIdGet(orgId: orgId, paymentId: paymentId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **paymentId** | **String** |  | 

### Return type

[**Payment**](Payment.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdPaymentsPaymentIdPut**
```swift
    open class func orgsOrgIdPaymentsPaymentIdPut(orgId: String, paymentId: String, payment: Payment, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Update payment

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let paymentId = "paymentId_example" // String | 
let payment = Payment(id: "id_example", organizationId: "organizationId_example", amount: 123, currency: "currency_example", description: "description_example") // Payment | 

// Update payment
DefaultAPI.orgsOrgIdPaymentsPaymentIdPut(orgId: orgId, paymentId: paymentId, payment: payment) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **paymentId** | **String** |  | 
 **payment** | [**Payment**](Payment.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **orgsOrgIdPaymentsPost**
```swift
    open class func orgsOrgIdPaymentsPost(orgId: String, payment: Payment, completion: @escaping (_ data: Void?, _ error: Error?) -> Void)
```

Create payment

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OptiOfficeSDK

let orgId = "orgId_example" // String | 
let payment = Payment(id: "id_example", organizationId: "organizationId_example", amount: 123, currency: "currency_example", description: "description_example") // Payment | 

// Create payment
DefaultAPI.orgsOrgIdPaymentsPost(orgId: orgId, payment: payment) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orgId** | **String** |  | 
 **payment** | [**Payment**](Payment.md) |  | 

### Return type

Void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

