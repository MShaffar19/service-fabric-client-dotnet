# Register-SFApplicationType
Provisions or registers a Service Fabric application type with the cluster using the '.sfpkg' package in the external store or using the application package in the image store.
## Description

Provisions a Service Fabric application type with the cluster. The provision is required before any new applications 
can be instantiated.
                The provision operation can be performed either on the application package specified by the 
relativePathInImageStore, or by using the URI of the external '.sfpkg'.



## Required Parameters
#### -ApplicationTypeBuildPath

The relative path for the application package in the image store specified during the prior upload operation.



#### -ApplicationPackageDownloadUri

The path to the '.sfpkg' application package from where the application package can be downloaded using HTTP or HTTPS 
protocols. The application package can be stored in an external store that provides GET operation to download the 
file. Supported protocols are HTTP and HTTPS, and the path must allow READ access.



#### -ApplicationTypeName

The application type name represents the name of the application type found in the application manifest.



#### -ApplicationTypeVersion

The application type version represents the version of the application type found in the application manifest.



## Optional Parameters
#### -Async

Indicates whether or not provisioning should occur asynchronously. When set to true, the provision operation returns 
when the request is accepted by the system, and the provision operation continues without any timeout limit. The 
default value is false. For large application packages, we recommend setting the value to true.



#### -ApplicationPackageCleanupPolicy

The kind of action that needs to be taken for cleaning up the application package after successful provision. Possible 
values include: 'Invalid', 'Default', 'Automatic', 'Manual'



#### -ServerTimeout

The server timeout for performing the operation in seconds. This timeout specifies the time duration that the client 
is willing to wait for the requested operation to complete. The default value for this parameter is 60 seconds.



