# Cloudmersive.APIClient.NET.DLP.Model.DlpAdvancedDocumentRedactionResponse
Response object for advanced DLP document redaction with 35 PII detection results, redacted document, and optional rationale.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RedactedDocument** | **byte[]** | The redacted document as a rasterized PDF with PII regions redacted, or the original file if no disallowed PII was found. | [optional] 
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
**ContainsHealthInsuranceMemberID** | **bool** | True if the document contains health insurance member IDs. | [optional] 
**ContainsHealthInjuryOrDisease** | **bool** | True if the document contains references to injuries or diseases. | [optional] 
**ContainsHealthTypeOfTreatment** | **bool** | True if the document contains references to types of medical treatment. | [optional] 
**ContainsHealthDateAndTimeOfTreatment** | **bool** | True if the document contains dates and times of medical treatment. | [optional] 
**ContainsHealthPlanBeneficiaryNumber** | **bool** | True if the document contains health plan beneficiary numbers. | [optional] 
**ContainsHealthPaymentsMadeForTreatment** | **bool** | True if the document contains payments made for medical treatment. | [optional] 
**ContainsFaces** | **bool** | True if the document contains identifiable human faces. | [optional] 
**ContainsVehicleID** | **bool** | True if the document contains vehicle identifiers (e.g. license plates, VINs). | [optional] 
**ContainsDeviceID** | **bool** | True if the document contains device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs). | [optional] 
**ContainsNamesOfRelatives** | **bool** | True if the document contains names of relatives. | [optional] 
**ContainsHealthUniversalRecordLocator** | **bool** | True if the document contains health universal record locators (URLs). | [optional] 
**ContainsBiometrics** | **bool** | True if the document contains biometric data references (e.g. fingerprints, retinal scans, voiceprints). | [optional] 
**PagesRedacted** | [**List&lt;RedactedPageInfo&gt;**](RedactedPageInfo.md) | List of pages that were redacted (had PII regions redacted). | [optional] 
**AnalysisRationale** | **string** | Rationale for why the conclusion was formed. Only populated when ProvideAnalysisRationale is set to true in the request. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

