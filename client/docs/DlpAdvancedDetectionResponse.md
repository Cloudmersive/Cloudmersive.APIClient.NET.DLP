# Cloudmersive.APIClient.NET.DLP.Model.DlpAdvancedDetectionResponse
Response object for advanced DLP text detection with 29 PII detection types including health-related data.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CleanResult** | **bool** | True if no disallowed PII or sensitive data types were detected in the input text; false if any disallowed type was found. | [optional] 
**ContainsEmailAddress** | **bool** | True if the input text contains email addresses. | [optional] 
**ContainsPhoneNumber** | **bool** | True if the input text contains phone numbers. | [optional] 
**ContainsStreetAddress** | **bool** | True if the input text contains street addresses. | [optional] 
**ContainsPersonName** | **bool** | True if the input text contains person names. | [optional] 
**ContainsBirthDate** | **bool** | True if the input text contains birth dates. | [optional] 
**ContainsPassportNumber** | **bool** | True if the input text contains passport numbers. | [optional] 
**ContainsDriversLicense** | **bool** | True if the input text contains drivers license numbers. | [optional] 
**ContainsSocialSecurityNumber** | **bool** | True if the input text contains social security numbers. | [optional] 
**ContainsTaxpayerID** | **bool** | True if the input text contains taxpayer IDs. | [optional] 
**ContainsCreditCardNumber** | **bool** | True if the input text contains credit card numbers. | [optional] 
**ContainsCreditCardExpirationDate** | **bool** | True if the input text contains credit card expiration dates. | [optional] 
**ContainsCreditCardVerificationCode** | **bool** | True if the input text contains credit card verification codes. | [optional] 
**ContainsBankAccountNumber** | **bool** | True if the input text contains bank account numbers. | [optional] 
**ContainsIBAN** | **bool** | True if the input text contains IBANs. | [optional] 
**ContainsHealthInsuranceNumber** | **bool** | True if the input text contains health insurance numbers. | [optional] 
**ContainsBearerToken** | **bool** | True if the input text contains bearer tokens. | [optional] 
**ContainsHttpCookie** | **bool** | True if the input text contains HTTP cookies. | [optional] 
**ContainsPrivateKeys** | **bool** | True if the input text contains private keys. | [optional] 
**ContainsCredentials** | **bool** | True if the input text contains credentials (usernames/passwords). | [optional] 
**ContainsDeepWebUrls** | **bool** | True if the input text contains deep web URLs (.onion). | [optional] 
**ContainsSourceCode** | **bool** | True if the input text contains source code. | [optional] 
**ContainsIpAddress** | **bool** | True if the input text contains IP addresses. | [optional] 
**ContainsMacAddress** | **bool** | True if the input text contains MAC addresses. | [optional] 
**ContainsHealthInsuranceMemberID** | **bool** | True if the input text contains health insurance member IDs. | [optional] 
**ContainsHealthInjuryOrDisease** | **bool** | True if the input text contains references to injuries or diseases. | [optional] 
**ContainsHealthTypeOfTreatment** | **bool** | True if the input text contains references to types of medical treatment. | [optional] 
**ContainsHealthDateAndTimeOfTreatment** | **bool** | True if the input text contains dates and times of medical treatment. | [optional] 
**ContainsHealthPlanBeneficiaryNumber** | **bool** | True if the input text contains health plan beneficiary numbers. | [optional] 
**ContainsHealthPaymentsMadeForTreatment** | **bool** | True if the input text contains payments made for medical treatment. | [optional] 
**ContainsFaces** | **bool** | True if the document contains identifiable human faces. | [optional] 
**ContainsVehicleID** | **bool** | True if the input contains vehicle identifiers (e.g. license plates, VINs). | [optional] 
**ContainsDeviceID** | **bool** | True if the input contains device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs). | [optional] 
**ContainsNamesOfRelatives** | **bool** | True if the input contains names of relatives. | [optional] 
**ContainsHealthUniversalRecordLocator** | **bool** | True if the input contains health universal record locators (URLs). | [optional] 
**ContainsBiometrics** | **bool** | True if the input contains biometric data references (e.g. fingerprints, retinal scans, voiceprints). | [optional] 
**AnalysisRationale** | **string** | Rationale for why the conclusion was formed. Only populated when ProvideAnalysisRationale is set to true in the request. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

