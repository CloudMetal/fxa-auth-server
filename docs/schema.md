
## SessionTokens

* id
* uid
* email
* emailCode
* verified

## KeyFetchTokens

* id
* uid
* kA
* wrapKb
* verified

## AccountResetTokens

* id
* uid

## AuthTokens

* id
* uid
* (for sessionToken)
	* email
	* emailCode
* (for keyFetchToken)
	* kA
	* wrapKb
* (for both)
	* verified

## SrpTokens

* id
* uid
* N
* g
* s
* v
* b
* B
* passwordStretching
* (for authToken)
	* email
	* emailCode
	* kA
	* wrapKb
	* verified

## ForgotPasswordTokens

* id
* uid
* email
* passcode
* ttl
* codeLength
* tries

## Emails

* email
* uid
* srp
* passwordStretching
* (for srpToken)
	* emailCode
	* kA
	* wrapKb
	* verified

## Accounts

* uid
* email
* emailCode
* sessionTokens
* keyFetchTokens
* srpTokens
* authTokens
* accountResetToken
* forgotPasswordToken
