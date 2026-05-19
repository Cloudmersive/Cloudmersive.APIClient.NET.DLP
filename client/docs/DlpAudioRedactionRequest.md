# Cloudmersive.APIClient.NET.DLP.Model.DlpAudioRedactionRequest
Request object for DLP audio redaction with 23 PII detection types.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InputFile** | **byte[]** | Audio file bytes (WAV, MP3, M4A, FLAC, OGG, or WMA) to transcribe, scan for PII, and redact. | [optional] 
**LanguageCode** | **string** | Language code for speech recognition. Default is \&quot;ENG\&quot; (English). | [optional] 
**AllowEmailAddress** | **bool** | Set to true to allow email addresses in the audio transcript and not redact them. | [optional] 
**AllowPhoneNumber** | **bool** | Set to true to allow phone numbers in the audio transcript and not redact them. | [optional] 
**AllowStreetAddress** | **bool** | Set to true to allow street addresses in the audio transcript and not redact them. | [optional] 
**AllowPersonName** | **bool** | Set to true to allow person names in the audio transcript and not redact them. | [optional] 
**AllowBirthDate** | **bool** | Set to true to allow birth dates in the audio transcript and not redact them. | [optional] 
**AllowPassportNumber** | **bool** | Set to true to allow passport numbers in the audio transcript and not redact them. | [optional] 
**AllowDriversLicense** | **bool** | Set to true to allow drivers license numbers in the audio transcript and not redact them. | [optional] 
**AllowSocialSecurityNumber** | **bool** | Set to true to allow social security numbers in the audio transcript and not redact them. | [optional] 
**AllowTaxpayerID** | **bool** | Set to true to allow taxpayer IDs in the audio transcript and not redact them. | [optional] 
**AllowCreditCardNumber** | **bool** | Set to true to allow credit card numbers in the audio transcript and not redact them. | [optional] 
**AllowCreditCardExpirationDate** | **bool** | Set to true to allow credit card expiration dates in the audio transcript and not redact them. | [optional] 
**AllowCreditCardVerificationCode** | **bool** | Set to true to allow credit card verification codes in the audio transcript and not redact them. | [optional] 
**AllowBankAccountNumber** | **bool** | Set to true to allow bank account numbers in the audio transcript and not redact them. | [optional] 
**AllowIBAN** | **bool** | Set to true to allow IBANs in the audio transcript and not redact them. | [optional] 
**AllowHealthInsuranceNumber** | **bool** | Set to true to allow health insurance numbers in the audio transcript and not redact them. | [optional] 
**AllowBearerToken** | **bool** | Set to true to allow bearer tokens in the audio transcript and not redact them. | [optional] 
**AllowHttpCookie** | **bool** | Set to true to allow HTTP cookies in the audio transcript and not redact them. | [optional] 
**AllowPrivateKeys** | **bool** | Set to true to allow private keys in the audio transcript and not redact them. | [optional] 
**AllowCredentials** | **bool** | Set to true to allow credentials (usernames/passwords) in the audio transcript and not redact them. | [optional] 
**AllowDeepWebUrls** | **bool** | Set to true to allow deep web URLs (.onion) in the audio transcript and not redact them. | [optional] 
**AllowSourceCode** | **bool** | Set to true to allow source code in the audio transcript and not redact it. | [optional] 
**AllowIpAddress** | **bool** | Set to true to allow IP addresses in the audio transcript and not redact them. | [optional] 
**AllowMacAddress** | **bool** | Set to true to allow MAC addresses in the audio transcript and not redact them. | [optional] 
**RedactionMode** | **string** | Redaction mode for audio: \&quot;Bleep\&quot; (default) replaces redacted audio segments with a bleep tone, or \&quot;Mute\&quot; zeroes out the audio for the redacted portions. | [optional] 
**TranscriptRedactionMode** | **string** | Redaction mode for the transcript text: \&quot;SemanticTag\&quot; (default) replaces PII with a semantic tag in square brackets (e.g. [PHONE-NUMBER]), \&quot;Delete\&quot; removes PII entirely, or \&quot;ReplaceWithAsterisk\&quot; replaces PII characters with asterisks (*). | [optional] 
**SpeechRecognitionMode** | **string** | Optional. Speech recognition mode used when transcribing the audio for redaction. Available values: \&quot;Fast\&quot;, \&quot;Normal\&quot;, or \&quot;Advanced\&quot;. Defaults to \&quot;Normal\&quot; when not specified. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

