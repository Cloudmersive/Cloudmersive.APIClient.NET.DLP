# Cloudmersive.APIClient.NET.DLP.Model.DlpDocumentRedactionResponse
Response object for DLP document redaction with 23 PII detection results and redacted document.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RedactedDocument** | **byte[]** | The redacted document as a rasterized PDF with PII regions blurred, or the original file if no disallowed PII was found. | [optional] 
**CleanResult** | **bool** | True if no disallowed PII or sensitive data types were detected; false if any disallowed type was found and redacted. | [optional] 
**ContainsEmailAddress** | **bool** | True if the document contains email addresses. | [optional] 
**ContainsPhoneNumber** | **bool** | True if the document contains phone numbers. | [optional] 
**ContainsStreetAddress** | **bool** | True if the document contains street addresses. | [optional] 
**ContainsPersonName** | **bool** | True if the document contains person names. | [optional] 
**ContainsBirthDate** | **bool** | True if the document contains birth dates. | [optional] 
**ContainsPassportNumber** | **bool** | True if the document contains passport numbers. | [optional] 
**ContainsDriversLicense** | **bool** | True if the document contains drivers license numbers. | [optional] 
**ContainsSocialSecurityNumber** | **bool** | True if the document contains social security numbers. | [optional] 
**ContainsTaxpayerID** | **bool** | True if the document contains taxpayer IDs. | [optional] 
**ContainsCreditCardNumber** | **bool** | True if the document contains credit card numbers. | [optional] 
**ContainsCreditCardExpirationDate** | **bool** | True if the document contains credit card expiration dates. | [optional] 
**ContainsCreditCardVerificationCode** | **bool** | True if the document contains credit card verification codes. | [optional] 
**ContainsBankAccountNumber** | **bool** | True if the document contains bank account numbers. | [optional] 
**ContainsIBAN** | **bool** | True if the document contains IBANs. | [optional] 
**ContainsHealthInsuranceNumber** | **bool** | True if the document contains health insurance numbers. | [optional] 
**ContainsBearerToken** | **bool** | True if the document contains bearer tokens. | [optional] 
**ContainsHttpCookie** | **bool** | True if the document contains HTTP cookies. | [optional] 
**ContainsPrivateKeys** | **bool** | True if the document contains private keys. | [optional] 
**ContainsCredentials** | **bool** | True if the document contains credentials (usernames/passwords). | [optional] 
**ContainsDeepWebUrls** | **bool** | True if the document contains deep web URLs (.onion). | [optional] 
**ContainsSourceCode** | **bool** | True if the document contains source code. | [optional] 
**ContainsIpAddress** | **bool** | True if the document contains IP addresses. | [optional] 
**ContainsMacAddress** | **bool** | True if the document contains MAC addresses. | [optional] 
**PagesRedacted** | [**List&lt;RedactedPageInfo&gt;**](RedactedPageInfo.md) | List of pages that were redacted (had PII regions blurred). | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

