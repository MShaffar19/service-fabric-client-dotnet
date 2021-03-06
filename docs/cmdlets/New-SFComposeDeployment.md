# New-SFComposeDeployment
Creates a Service Fabric compose deployment.
## Description

Compose is a file format that describes multi-container applications. This API allows deploying container based 
applications defined in compose format in a Service Fabric cluster. Once the deployment is created, its status can be 
tracked via the `GetComposeDeploymentStatus` API.



## Required Parameters
#### -DeploymentName

The name of the deployment.



#### -ComposeFileContent

The content of the compose file that describes the deployment to create.



## Optional Parameters
#### -RegistryUserName

The user name to connect to container registry.



#### -RegistryPassword

The password for supplied username to connect to container registry.



#### -PasswordEncrypted

Indicates that supplied container registry password is encrypted.



#### -ServerTimeout

The server timeout for performing the operation in seconds. This timeout specifies the time duration that the client 
is willing to wait for the requested operation to complete. The default value for this parameter is 60 seconds.



