# Lark IT Ansible AWS KMS Role

Create customer managed KMS key

## Dependencies
This role is not dependent on any other roles

## Variables
| Variable | Required? | Default Value | Type | Description |
|----------|-----------|---------------|------|-------------|
| kms_cmk_name | Yes | N/A | String | KMS CMK name |
| kms_cmk_purpose | Yes | N/A | String | KMS CMK purpose or description |
| kms_grant_required | No | false | Boolean | Set to true to define a KMS Grant |
| kms_grantee_operations | When kms_grant_required = true | N/A | String | The opreations the grantee is allowed to perform on the key |
| aws_account_id | When kms_grant_required = true | N/A | String | The AWS account id of the grantee |
| kms_grantee_principal_type | When kms_grant_required = true | N/A | String | The grantee principal type |
| kms_grantee_principal_name | When kms_grant_required = true | N/A | String | The name of the grantee principal |