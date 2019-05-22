# okta_app_flow

This is a sample module which integrates the application registration process with Okta. You will need access to the Okta Management API (access token), see https://developer.okta.com/docs/api/getting_started/getting_a_token for details.

The flow of the application registration is as:
1. Create Application in Apigee Edge and generate client id & client secret
2. Module calls Okta to register Application with client id & client secret

To install this module please drop it in sites/all/modules/custom folder

To configure Drupal portal to use the module:
1. Login as an administrator
2. Navigate to module administration
3. Search for "Okta App Creation Custom Workflow" and enable it
4. Navigate top menu "Configuration > Administration > Okta External Application Registration"
5. Input your own Okta server endpoint and SSWS Token
