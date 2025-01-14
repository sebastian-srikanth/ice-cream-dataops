# ex. cdf-bootcamp-01-test
CDF_PROJECT=sebastian-srikanth
LOGIN_FLOW=client_credentials

# Client Ids and Client Secrets are identifiers for App registrations/Service Principals
# ex. xxxxxxx-xxxx-xxxx-xxxxxxxxxxxx
IDP_CLIENT_ID=14c959b2-4df6-49b0-bcf6-81e95b177e02
# ex. xfgFXG~ugf8rfui322fg
IDP_CLIENT_SECRET=ZwX8Q~QkN5c1SbPCLtBYGV.KyOZeJjwd2cazLaEZ

# ex. xxxxxxx-xxxx-xxxx-xxxxxxxxxxxx
DATA_PIPELINE_OEE_CLIENT_ID=14c959b2-4df6-49b0-bcf6-81e95b177e02
# # ex. xfgFXG~ugf8rfui322fg
DATA_PIPELINE_OEE_CLIENT_SECRET=ZwX8Q~QkN5c1SbPCLtBYGV.KyOZeJjwd2cazLaEZ

# # ex. xxxxxxx-xxxx-xxxx-xxxxxxxxxxxx
ICAPI_EXTRACTORS_CLIENT_ID=14c959b2-4df6-49b0-bcf6-81e95b177e02
# # ex. xfgFXG~ugf8rfui322fg
ICAPI_EXTRACTORS_CLIENT_SECRET=ZwX8Q~QkN5c1SbPCLtBYGV.KyOZeJjwd2cazLaEZ

# Note: If you use Microsoft Entra ID as your IdP, you only need to specify the ID for your Entra ID tenant by replacing IDP_TOKEN_URL with IDP_TENANT_ID. However, leave both in as the extractors require this environment variable.
IDP_TENANT_ID=d4febcbc-db24-4823-bffd-92fd05b9c6bc # All bootcamp projects share the same tenant.
IDP_TOKEN_URL=https://login.microsoftonline.com/d4febcbc-db24-4823-bffd-92fd05b9c6bc/oauth2/v2.0/token

# The below variables are the defaults, they are automatically constructed unless they are set.
CDF_URL=https://bluefield.cognitedata.com
IDP_SCOPES=https://bluefield.cognitedata.com/.default
CDF_CLUSTER=bluefield

