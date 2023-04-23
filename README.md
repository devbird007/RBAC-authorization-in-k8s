# RBAC-authorization-in-k8s
This repository contains a couple of examples demonstrating how to manage users and group
access to kubernetes resources with RBAC.
You can create the following components
* Role: This defines access permissions within a namespace in a cluster.
* RoleBinding: This component is how you link a Role to users and groups.
* ClusterRole: This lets you define access permissions across the entire cluster,
as opposed to being limited to a specific namespace.
* ClusterRoleBinding: This component is how you link a ClusterRole to users and groups.
* ServiceAccounts: This lets you create users for applications that need access
to various resources. With the ServiceAccount component, applications can then be connected to
Roles and ClusterRoles.

Kubernetes doesn't natively support the creation and management of users, it relies on
external sources for authentication. These are:
* Static Token File
* Certificates
* 3rd party Identity Services

Once these users and groups are created and defined, they can then be connected to your
cluster with the components listed above.
