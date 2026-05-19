# Cloudmersive.APIClient.NET.DLP.Model.DlpAdvancedAudioDetectionRequest
Request object for advanced DLP audio detection with 29 PII detection types including health-related data.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InputFile** | **byte[]** | Audio file bytes (WAV, MP3, M4A, FLAC, OGG, or WMA) to transcribe and scan for PII and sensitive data. | [optional] 
**LanguageCode** | **string** | Language code for speech recognition. Default is \&quot;ENG\&quot; (English). | [optional] 
**AllowEmailAddress** | **bool** | Set to true to allow email addresses in the audio transcript and not flag them as PII. | [optional] 
**AllowPhoneNumber** | **bool** | Set to true to allow phone numbers in the audio transcript and not flag them as PII. | [optional] 
**AllowStreetAddress** | **bool** | Set to true to allow street addresses in the audio transcript and not flag them as PII. | [optional] 
**AllowCity** | **bool** | Set to true to allow standalone city names (e.g. \&quot;San Francisco\&quot;) in the audio transcript and not flag them as PII. Applies to city names mentioned outside of a full street address. | [optional] 
**AllowPersonName** | **bool** | Set to true to allow person names in the audio transcript and not flag them as PII. | [optional] 
**AllowBirthDate** | **bool** | Set to true to allow birth dates in the audio transcript and not flag them as PII. | [optional] 
**AllowPassportNumber** | **bool** | Set to true to allow passport numbers in the audio transcript and not flag them as PII. | [optional] 
**AllowDriversLicense** | **bool** | Set to true to allow drivers license numbers in the audio transcript and not flag them as PII. | [optional] 
**AllowSocialSecurityNumber** | **bool** | Set to true to allow social security numbers in the audio transcript and not flag them as PII. | [optional] 
**AllowTaxpayerID** | **bool** | Set to true to allow taxpayer IDs in the audio transcript and not flag them as PII. | [optional] 
**AllowCreditCardNumber** | **bool** | Set to true to allow credit card numbers in the audio transcript and not flag them as PII. | [optional] 
**AllowCreditCardExpirationDate** | **bool** | Set to true to allow credit card expiration dates in the audio transcript and not flag them as PII. | [optional] 
**AllowCreditCardVerificationCode** | **bool** | Set to true to allow credit card verification codes in the audio transcript and not flag them as PII. | [optional] 
**AllowBankAccountNumber** | **bool** | Set to true to allow bank account numbers in the audio transcript and not flag them as PII. | [optional] 
**AllowIBAN** | **bool** | Set to true to allow IBANs in the audio transcript and not flag them as PII. | [optional] 
**AllowHealthInsuranceNumber** | **bool** | Set to true to allow health insurance numbers in the audio transcript and not flag them as PII. | [optional] 
**AllowBearerToken** | **bool** | Set to true to allow bearer tokens in the audio transcript and not flag them as PII. | [optional] 
**AllowHttpCookie** | **bool** | Set to true to allow HTTP cookies in the audio transcript and not flag them as PII. | [optional] 
**AllowPrivateKeys** | **bool** | Set to true to allow private keys in the audio transcript and not flag them as PII. | [optional] 
**AllowCredentials** | **bool** | Set to true to allow credentials (usernames/passwords) in the audio transcript and not flag them as PII. | [optional] 
**AllowDeepWebUrls** | **bool** | Set to true to allow deep web URLs (.onion) in the audio transcript and not flag them as PII. | [optional] 
**AllowSourceCode** | **bool** | Set to true to allow source code in the audio transcript and not flag it as sensitive data. | [optional] 
**AllowIpAddress** | **bool** | Set to true to allow IP addresses in the audio transcript and not flag them as PII. | [optional] 
**AllowMacAddress** | **bool** | Set to true to allow MAC addresses in the audio transcript and not flag them as PII. | [optional] 
**AllowHealthInsuranceMemberID** | **bool** | Set to true to allow health insurance member IDs in the audio transcript and not flag them as PHI. | [optional] 
**AllowMedicalRecordNumber** | **bool** | Set to true to allow medical record numbers in the audio transcript and not flag them as PHI. | [optional] 
**AllowBillingAccountNumber** | **bool** | Set to true to allow billing account numbers (e.g. provider/customer billing account IDs, distinct from bank account numbers) in the audio transcript and not flag them as PII. | [optional] 
**AllowHealthInjuryOrDisease** | **bool** | Set to true to allow references to injuries or diseases in the audio transcript and not flag them as PHI. | [optional] 
**AllowHealthTypeOfTreatment** | **bool** | Set to true to allow references to types of medical treatment in the audio transcript and not flag them as PHI. | [optional] 
**AllowHealthDateAndTimeOfTreatment** | **bool** | Set to true to allow dates and times of medical treatment in the audio transcript and not flag them as PHI. | [optional] 
**AllowHealthPlanBeneficiaryNumber** | **bool** | Set to true to allow health plan beneficiary numbers in the audio transcript and not flag them as PHI. | [optional] 
**AllowHealthPaymentsMadeForTreatment** | **bool** | Set to true to allow payments made for medical treatment in the audio transcript and not flag them as PHI. | [optional] 
**AllowVehicleID** | **bool** | Set to true to allow vehicle identifiers (e.g. license plates, VINs) in the audio transcript and not flag them as PII. | [optional] 
**AllowDeviceID** | **bool** | Set to true to allow device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs) in the audio transcript and not flag them as PII. | [optional] 
**AllowNamesOfRelatives** | **bool** | Set to true to allow names of relatives in the audio transcript and not flag them as PII. | [optional] 
**AllowHealthUniversalRecordLocator** | **bool** | Set to true to allow health universal record locators (URLs) in the audio transcript and not flag them as PHI. | [optional] 
**AllowBiometrics** | **bool** | Set to true to allow biometric data references (e.g. fingerprints, retinal scans, voiceprints) in the audio transcript and not flag them as PII. | [optional] 
**ProvideAnalysisRationale** | **bool** | Set to true to include a natural language rationale explaining why each detection conclusion was formed. | [optional] 
**CustomPolicyID** | **string** | Apply a Custom Policy for DLP Enforcement by providing the ID; to create a Custom Policy,  navigate to the Cloudmersive Management Portal and select Custom Policies.  Requires Managed Instance or Private Cloud | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

