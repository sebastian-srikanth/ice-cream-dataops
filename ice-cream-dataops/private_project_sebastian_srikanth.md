environment:
  name: test
  project: sebastian-srikanth
  type: test
  selected:
  - modules/bootcamp/data_foundation
  - modules/bootcamp/ice_cream_api
  - modules/bootcamp/use_cases/oee

variables:
  modules:
    bootcamp:
      CDF_PROJECT: sebastian-srikanth # ex. cdf-bootcamp-01-test
      IDP_CLIENT_ID: ${IDP_CLIENT_ID} # replaced by .env
      IDP_CLIENT_SECRET: ${IDP_CLIENT_SECRET} # replaced by .env
      IDP_TENANT_ID: ${IDP_TENANT_ID} # replaced by .env
      IDP_SCOPES: ${IDP_SCOPES} # replaced by .env
      # This is related to the cluster where the CDF project is hosted.
      CDF_URL: ${CDF_URL} # replaced by .env
      CDF_CLUSTER: bluefield
      IDP_TOKEN_URL: ${IDP_TOKEN_URL} # replaced by .env
      # Groups
      # OBJECT ID FOR TEST/PROD DATA PIPELINE OEE ENTRA GROUP
      data_developer_source_id: badb5a69-5198-4653-9214-a71e9794f28f
      data_pipeline_oee_source_id: badb5a69-5198-4653-9214-a71e9794f28f
      # OBJECT ID FOR TEST/PROD ADMIN TK ENTRA GROUP
      readwrite_source_id: badb5a69-5198-4653-9214-a71e9794f28f
      # OBJECT ID FOR TEST/PROD ADMIN TK ENTRA GROUP
      readonly_source_id: badb5a69-5198-4653-9214-a71e9794f28f
      # OBJECT ID FOR TEST/PROD ICAPI EXTRACTORS ENTRA GROUP
      icapi_extractors_source_id: badb5a69-5198-4653-9214-a71e9794f28f
      # Client Ids
      data_pipeline_oee_client_id: ${DATA_PIPELINE_OEE_CLIENT_ID} # replaced by .env
      data_pipeline_oee_client_secret: ${DATA_PIPELINE_OEE_CLIENT_SECRET} # replaced by .env
      icapi_extractors_client_id: ${ICAPI_EXTRACTORS_CLIENT_ID} # replaced by .env
      icapi_extractors_client_secret: ${ICAPI_EXTRACTORS_CLIENT_SECRET} # replaced by .env
      # Variables shared by modules
      icapi_ds_external_id: ds_icapi
      use_cases:
        oee:
          uc_oee_ds_external_id: ds_uc_oee