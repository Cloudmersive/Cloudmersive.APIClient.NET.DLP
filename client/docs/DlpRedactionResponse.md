# Cloudmersive.APIClient.NET.DLP.Model.DlpRedactionResponse
Response object for DLP text redaction with 23 PII detection results and redacted text.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RedactedText** | **string** | The redacted text with PII removed or replaced, or the original text if no disallowed PII was found. | [optional] 
**CleanResult** | **bool** | True if no disallowed PII or sensitive data types were detected; false if any disallowed type was found and redacted. | [optional] 
**ContainsEmailAddress** | **bool** | True if the input contains email addresses. | [optional] 
**ContainsPhoneNumber** | **bool** | True if the input contains phone numbers. | [optional] 
**ContainsStreetAddress** | **bool** | True if the input contains street addresses. | [optional] 
**ContainsPersonName** | **bool** | True if the input contains person names. | [optional] 
**ContainsBirthDate** | **bool** | True if the input contains birth dates. | [optional] 
**ContainsPassportNumber** | **bool** | True if the input contains passport numbers. | [optional] 
**ContainsDriversLicense** | **bool** | True if the input contains drivers license numbers. | [optional] 
**ContainsSocialSecurityNumber** | **bool** | True if the input contains social security numbers. | [optional] 
**ContainsTaxpayerID** | **bool** | True if the input contains taxpayer IDs. | [optional] 
**ContainsCreditCardNumber** | **bool** | True if the input contains credit card numbers. | [optional] 
**ContainsCreditCardExpirationDate** | **bool** | True if the input contains credit card expiration dates. | [optional] 
**ContainsCreditCardVerificationCode** | **bool** | True if the input contains credit card verification codes. | [optional] 
**ContainsBankAccountNumber** | **bool** | True if the input contains bank account numbers. | [optional] 
**ContainsIBAN** | **bool** | True if the input contains IBANs. | [optional] 
**ContainsHealthInsuranceNumber** | **bool** | True if the input contains health insurance numbers. | [optional] 
**ContainsBearerToken** | **bool** | True if the input contains bearer tokens. | [optional] 
**ContainsHttpCookie** | **bool** | True if the input contains HTTP cookies. | [optional] 
**ContainsPrivateKeys** | **bool** | True if the input contains private keys. | [optional] 
**ContainsCredentials** | **bool** | True if the input contains credentials (usernames/passwords). | [optional] 
**ContainsDeepWebUrls** | **bool** | True if the input contains deep web URLs (.onion). | [optional] 
**ContainsSourceCode** | **bool** | True if the input contains source code. | [optional] 
**ContainsIpAddress** | **bool** | True if the input contains IP addresses. | [optional] 
**ContainsMacAddress** | **bool** | True if the input contains MAC addresses. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

