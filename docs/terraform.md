## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| attributes | Additional attributes (_e.g._ "1") | list | `<list>` | no |
| capabilities | A list of capabilities. Valid values: CAPABILITY_IAM, CAPABILITY_NAMED_IAM, CAPABILITY_AUTO_EXPAND | list | `<list>` | no |
| delimiter | Delimiter between `name`, `namespace`, `stage` and `attributes` | string | `-` | no |
| enabled | Set to false to prevent the module from creating any resources | string | `true` | no |
| executor_role_name | Name of the IAM Role in all target accounts for Stack Set operations | string | `AWSCloudFormationStackSetExecutionRole` | no |
| name | Name | string | `cis` | no |
| namespace | Namespace (e.g. `cp` or `cloudposse`) | string | - | yes |
| parameters | Key-value map of input parameters for the Stack Set template. (_e.g._ map("BusinessUnit","ABC") | map | `<map>` | no |
| stage | Stage (e.g. `prod`, `dev`, `staging`) | string | - | yes |
| tags | Additional tags (_e.g._ map("BusinessUnit","ABC") | map | `<map>` | no |
| template_url | Amazon S3 bucket URL location of a file containing the CloudFormation template body. Maximum file size: 460,800 bytes | string | - | yes |

## Outputs

| Name | Description |
|------|-------------|
| administrator_role_arn | Amazon Resource Number (ARN) of the IAM Role in the administrator account |
| executor_role_name | Name of the IAM Role in all target accounts for Stack Set operations |
| name | Name of the Stack Set |

