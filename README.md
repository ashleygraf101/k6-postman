# Exploratory API testing
Exploratory API testing with Postman and the test-k6 API.

TODO: Move most of the pre-request scripts from pre-test to pre-collection

TODO: add idempotent GET, DELETE, POST, PUT & PATCH tests

## Tests
- Register account
- Login basic auth
- Login token auth
- Register with all valid Params
- Register with no Params
- Register with already-used username
- Register with invalid username
- View list of public crocodiles
- View List of my crocodiles in invalid Accept format
- View one public crocodile
- View list of my crocodiles
- View one of my crocodiles
- Edit one of my crocodiles 
- Delete one of my crocodiles
- Create a crocodile with invalid date format
- Create a crocodile with required value as null
- Create a crocodile with non-accepted sex
- Create a crocodile with a too-long name
- Create names with formats that resemble name patterns found around the world (run alongside names.csv as k6-Names)
- Create a crocodile with naughty-string name (run alongside naughty-strings.csv as k6-Base64)
- View private crocodile that is not my crocodile
- Edit private crocodile that is not my crocodile
- Delete private crocodile that is not my crocodile
- Change a random private crocodile's characteristics
- Change a random private crocodile's characteristics with required field as null

## How to use
- go to test-k6 and create an account to use for the private crocodiles
- for STN, add environmental variables base_url, mock_server, and api_key
- for k6, create test-k6 account, then add environment variables base_url, testk6Token, testk6Username, testk6Passord, and authorization
- Import into Postman

## Postman Features used
- Environment
- Dynamic Variables
- custom variables
- Pre-request scripts
- "Post-request" scripts in Tests
