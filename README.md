# ![LOGO](logo.png) PolicyClient **flow**ground Connector

## Description

A generated **flow**ground connector for the PolicyClient API (version 2016-04-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/resources-policy/2016-04-01/swagger.json<br/>
Generated at: 2019-06-11T18:14:12+03:00

## API Description

To manage and control access to your resources, you can define customized policies and assign them at a scope.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets all the policy assignments for a subscription.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply on the operation.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets all the policy definitions for a subscription.

*Tags:* `PolicyDefinitions`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply on the operation.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Deletes a policy definition.

*Tags:* `PolicyDefinitions`

#### Input Parameters
* `policyDefinitionName` - _required_ - The name of the policy definition to delete.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets the policy definition.

*Tags:* `PolicyDefinitions`

#### Input Parameters
* `policyDefinitionName` - _required_ - The name of the policy definition to get.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Creates or updates a policy definition.

*Tags:* `PolicyDefinitions`

#### Input Parameters
* `policyDefinitionName` - _required_ - The name of the policy definition to create.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets policy assignments for the resource group.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group that contains policy assignments.
* `$filter` - _optional_ - The filter to apply on the operation.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets policy assignments for a resource.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group containing the resource. The name is case insensitive.
* `resourceProviderNamespace` - _required_ - The namespace of the resource provider.
* `parentResourcePath` - _required_ - The parent resource path.
* `resourceType` - _required_ - The resource type.
* `resourceName` - _required_ - The name of the resource with policy assignments.
* `$filter` - _optional_ - The filter to apply on the operation.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Deletes a policy assignment by ID.

> When providing a scope for the assignment, use '/subscriptions/{subscription-id}/' for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}' for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}' for resources.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `policyAssignmentId` - _required_ - The ID of the policy assignment to delete. Use the format '/{scope}/providers/Microsoft.Authorization/policyAssignments/{policy-assignment-name}'.
* `api-version` - _required_ - The API version to use for the operation.

### Gets a policy assignment by ID.

> When providing a scope for the assignment, use '/subscriptions/{subscription-id}/' for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}' for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}' for resources.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `policyAssignmentId` - _required_ - The ID of the policy assignment to get. Use the format '/{scope}/providers/Microsoft.Authorization/policyAssignments/{policy-assignment-name}'.
* `api-version` - _required_ - The API version to use for the operation.

### Creates a policy assignment by ID.

> Policy assignments are inherited by child resources. For example, when you apply a policy to a resource group that policy is assigned to all resources in the group. When providing a scope for the assignment, use '/subscriptions/{subscription-id}/' for subscriptions, '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}' for resource groups, and '/subscriptions/{subscription-id}/resourceGroups/{resource-group-name}/providers/{resource-provider-namespace}/{resource-type}/{resource-name}' for resources.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `policyAssignmentId` - _required_ - The ID of the policy assignment to create. Use the format '/{scope}/providers/Microsoft.Authorization/policyAssignments/{policy-assignment-name}'.
* `api-version` - _required_ - The API version to use for the operation.

### Deletes a policy assignment.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the policy assignment.
* `policyAssignmentName` - _required_ - The name of the policy assignment to delete.
* `api-version` - _required_ - The API version to use for the operation.

### Gets a policy assignment.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the policy assignment.
* `policyAssignmentName` - _required_ - The name of the policy assignment to get.
* `api-version` - _required_ - The API version to use for the operation.

### Creates a policy assignment.

> Policy assignments are inherited by child resources. For example, when you apply a policy to a resource group that policy is assigned to all resources in the group.

*Tags:* `PolicyAssignments`

#### Input Parameters
* `scope` - _required_ - The scope of the policy assignment.
* `policyAssignmentName` - _required_ - The name of the policy assignment.
* `api-version` - _required_ - The API version to use for the operation.

## License

**flow**ground :- Telekom iPaaS / azure-com-resources-policy-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
