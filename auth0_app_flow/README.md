# auth0_app_flow

This is a sample module which integrates the application registration process with Auth0. You will need access to the Auth0 Management API (access token), see https://auth0.com/docs/api/management/v2/get-access-tokens-for-test for details.

The flow of the application registration is as:
1. Create Application in Apigee Edge
2. Module calls Auth0 to register Application
3. Create new key for application in Apigee Edge with Auth0's returned client id/secret
4. Delete old client id/secret in Apigee Edge

To install this module please drop it in sites/all/modules/custom folder

To configure Drupal portal to use the module:
1. Login as an administrator
2. Navigate to module administration
3. Search for "Auth0 App Creation Custom Workflow" and enable it
4. Navigate top menu "Configuration > Administration > Auth0 External Application Registration"
5. Input your own Auth0 server endpoint and Bearer Token
