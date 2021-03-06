swagger: "2.0"
x-collection-name: Allied Irish Bank
x-complete: 1
info:
  title: Allied Irish Bank
  description: this-is-an-openapi-definition-for-the-standard-set-of-open-banking-httpopenbankingapis-io-apis-covering-the-allied-irish-bank-apis-
  termsOfService: https://www.openbanking.org.uk/open-licence/
  contact:
    name: API Evangelist
    url: https://apievangelist.com
    email: info@apievangelist.com
  version: 1.0.0
basePath: open-banking/v2.1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/direct-debits:
    get:
      summary: Get Account Direct Debits
      description: Get Direct Debits related to an account
      operationId: GetAccountDirectDebits
      x-api-path-slug: accountsaccountiddirectdebits-get
      parameters:
      - in: path
        name: AccountId
        description: A unique identifier used to identify the account resource
      - in: header
        name: Authorization
        description: An Authorisation Token as per https://tools
      - in: header
        name: x-fapi-customer-ip-address
        description: The PSUs IP address if the PSU is currently logged in with the
          TPP
      - in: header
        name: x-fapi-customer-last-logged-time
        description: The time when the PSU last logged in with the TPP
      - in: header
        name: x-fapi-financial-id
        description: The unique id of the ASPSP to which the request is issued
      - in: header
        name: x-fapi-interaction-id
        description: An RFC4122 UID used as a correlation id
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Account
      - Direct
      - Debits
  /direct-debits:
    get:
      summary: Get Direct Debits
      description: Get Direct Debits
      operationId: GetDirectDebits
      x-api-path-slug: directdebits-get
      parameters:
      - in: header
        name: Authorization
        description: An Authorisation Token as per https://tools
      - in: header
        name: x-fapi-customer-ip-address
        description: The PSUs IP address if the PSU is currently logged in with the
          TPP
      - in: header
        name: x-fapi-customer-last-logged-time
        description: The time when the PSU last logged in with the TPP
      - in: header
        name: x-fapi-financial-id
        description: The unique id of the ASPSP to which the request is issued
      - in: header
        name: x-fapi-interaction-id
        description: An RFC4122 UID used as a correlation id
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Direct
      - Debits
host: openapi.aibgb.co.uk