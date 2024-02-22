<!--


  ** DO NOT EDIT THIS FILE
  **
  ** 1) Make all changes to `README.yaml`
  ** 2) Run`make readme` to rebuild this file.
  **
  ** (We maintain HUNDREDS of open source projects. This is how we maintain our sanity.)
  **


  -->

# terraform-aws-workspaces

[![Build Status](https://travis-ci.org/hadenlabs/terraform-aws-workspaces.svg?branch=main)](https://travis-ci.org/hadenlabs/terraform-aws-workspaces) [![Latest Release](https://img.shields.io/github/release/hadenlabs/terraform-aws-workspaces.svg)](https://travis-ci.org/hadenlabs/terraform-aws-workspaces/releases)

Terraform module to provision an workspace instance.

---

This project is part of our comprehensive [hadenlabs](https://hadenlabs.com) modules of terraform.

It's 100% Open Source and licensed under the [APACHE2](LICENSE).

## Usage

```hcl
  module "main" {
    source  = "hadenlabs/workspaces/aws"
    version = "0.1.0"

    providers = {
      aws = aws.main
    }

  }
```

Full working example can be found in [example](./example) folder.

## Examples

### common

```hcl

  module "main" {
    source  = "hadenlabs/workspaces/aws"
    version = "0.1.0"

    providers = {
      aws = aws.main
    }
  }

```

 <!-- DO NOT EDIT. THIS FILE IS GENERATED BY THE MAKEFILE. -->

# Terraform variables

This document gives an overview of variables used in the platform of the terraform-aws-workspaces.

## Requirements

| Name      | Version |
| --------- | ------- |
| terraform | >= 0.13 |

## Providers

| Name | Version |
| ---- | ------- |
| aws  | n/a     |

## Inputs

| Name | Description | Type | Default | Required |
| --- | --- | --- | --- | :-: |
| bundle_id | id of bunlde | `string` | `"wsb-bh8rsxt14"` | no |
| create_directory | Create managed AWS AD/AD Connector | `bool` | `true` | no |
| directory_edition | If MicrosoftAD, select either Standard or Enterprise | `string` | `"Standard"` | no |
| directory_name | Directory Name (DNS name) | `string` | `"org.hadenlabs.com"` | no |
| directory_pass | password for directory | `string` | n/a | yes |
| directory_size | Directory Size. If SimpleAD or AD Connector, select either Small or Large. | `string` | `"Small"` | no |
| directory_type | Type of Directory to create. Options: SimpleAD, ADConnector or MicrosoftAD | `string` | `"MicrosoftAD"` | no |
| root_volume_encryption_enabled | This root volume encryption enabled | `bool` | `true` | no |
| tags | This is to help you add tags to your cloud objects | `map(any)` | `null` | no |
| update_dhcp_options | Use AD DNS servers to resolve queries on VPC | `bool` | `true` | no |
| user_name | name user for directory | `string` | `"Administrator"` | no |
| user_volume_encryption_enabled | This user volume encryption enabled | `bool` | `true` | no |
| volume_encryption_key | key for encryption volume | `string` | `"alias/aws/workspaces"` | no |

## Outputs

| Name      | Description   |
| --------- | ------------- |
| directory | The directory |
| workspace | The workspace |

## Help

**Got a question?**

File a GitHub [issue](https://github.com/hadenlabs/terraform-aws-workspaces/issues), send us an [email][email] or join our [Slack Community][slack].

## Contributing

### Bug Reports & Feature Requests

Please use the [issue tracker](https://github.com/hadenlabs/terraform-aws-workspaces/issues) to report any bugs or file feature requests.

### Developing

If you are interested in being a contributor and want to get involved in developing this project or [help out](https://hadenlabs.com) with our other projects, we would love to hear from you! Shoot us an [email](mailto:support@hadenlabs.com).

In general, PRs are welcome. We follow the typical "fork-and-pull" Git workflow.

1.  **Fork** the repo on GitHub
2.  **Clone** the project to your own machine
3.  **Commit** changes to your own branch
4.  **Push** your work back up to your fork
5.  Submit a **Pull Request** so that we can review your changes

**NOTE:** Be sure to rebase the latest changes from "upstream" before making a pull request!

### Versioning

Releases are managed using github release feature. We use \[Semantic Versioning\](<http://semver.org>) for all the releases. Every change made to the code base will be referred to in the release notes (except for cleanups and refactorings).

## Copyright

Copyright © 2018-2021 [Hadenlabs](https://hadenlabs.com)

## License

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

See [LICENSE](LICENSE) for full details.

    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

      https://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.

## Trademarks

All other trademarks referenced herein are the property of their respective owners.

## About

This project is maintained and funded by [Hadenlabs][https://hadenlabs.com]. Like it? Please let us know at <support@hadenlabs.com>

### Contributors

| [![Luis Mayta][luismayta_avatar]][luismayta_homepage]<br/>[Luis Mayta][luismayta_homepage] |
| ------------------------------------------------------------------------------------------ |

[luismayta_homepage]: https://github.com/luismayta
[luismayta_avatar]: https://github.com/luismayta.png?size=150
extra line
