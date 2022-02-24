---
page_type: sample
languages:
- csharp
products:
- service connector
description: "Sample projects to connect Azure WebApp to App Configuration via Service Connector"
urlFragment: "serviceconnector-webapp-appconfig-samples"
---

# Connect Azure WebApp to App Configuration via ServiceConnector
<!-- 
Guidelines on README format: https://review.docs.microsoft.com/help/onboard/admin/samples/concepts/readme-template?branch=master

Guidance on onboarding samples to docs.microsoft.com/samples: https://review.docs.microsoft.com/help/onboard/admin/samples/process/onboarding?branch=master

Taxonomies for products and languages: https://review.docs.microsoft.com/new-hope/information-architecture/metadata/taxonomies?branch=master
-->

## Overview
[Service Connector](https://docs.microsoft.com/en-us/azure/service-connector/) is an Azure-managed service that helps developers easily connect compute service to target backing services. This service configures the network settings and connection information (for example, generating environment variables) between compute service and target backing service. Developers just use preferred SDK or library that consumes the connection information to do data plane operations against target backing service.

Service Connector supports Azure WebApp, Azure Spring Cloud as source of connection, and over [10+ Azure services](https://docs.microsoft.com/en-us/azure/service-connector/overview#what-services-are-supported-in-service-connector) as target, such as PostgreSQL, MySQL, Storage, Keyvault, ServiceBus, SignalR etc.

This repository contains sample projects to connect Azure WebApp to App Configuration via ServiceConnector. 

## Sample list and How to Run
Below table shows the list of samples in this repository. All authentication types between Azure WebApp and App Configuration are covered.
| Folder name/How to Run |  Description |
|-------------|-----------------------------|
|[system-managed-identity](./webapp-keyvault-java) | Sample of connecting Azure WebApp hosting DotNet application to AppConfig with **system Managed Identity**|
|[user-assigned-managed-identity](./webapp-keyvault-java)| Sample of connecting Azure WebApp hosting DotNet application to AppConfig with **user assigned Managed Identity**|
|[service-principal](./webapp-keyvault-java)| Sample of connecting Azure WebApp hosting DotNet application to AppConfig with **service principal**|
|[access-key](./webapp-keyvault-java)| Sample of connecting Azure WebApp hosting DotNet application to AppConfig with **access key**|

## Useful References
- More samples to connect Azure WebApp with other target services, pls refer to [todo](todo).
- [ServiceConnector docs](todo)
- [FAQ](todo)

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


## License

Copyright (c) Microsoft Corporation. All rights reserved.

Licensed under the [MIT](./LICENSE) license.