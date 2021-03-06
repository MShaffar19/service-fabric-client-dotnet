# Get-SFComposeDeploymentStatusList
Gets the list of compose deployments created in the Service Fabric cluster.
## Description

Gets the status about the compose deployments that were created or in the process of being created in the Service 
Fabric cluster. The response includes the name, status, and other details about the compose deployments. If the list 
of deployments do not fit in a page, one page of results is returned as well as a continuation token, which can be 
used to get the next page.



## Optional Parameters
#### -MaxResults

The maximum number of results to be returned as part of the paged queries. This parameter defines the upper bound on 
the number of results returned. The results returned can be less than the specified maximum results if they do not fit 
in the message as per the max message size restrictions defined in the configuration. If this parameter is zero or not 
specified, the paged query includes as many results as possible that fit in the return message.



#### -ServerTimeout

The server timeout for performing the operation in seconds. This timeout specifies the time duration that the client 
is willing to wait for the requested operation to complete. The default value for this parameter is 60 seconds.



