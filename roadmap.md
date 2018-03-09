# VS Connected Environment Roadmap
VSCE is an Azure developer service that enables a fast, iterative development experience for Kubernetes. Teams can work within the same Connected Environment, and test code end-to-end without simulating or mocking dependencies.

This list shows what's on our 3-6 month radar for consideration and prioritization. It is not a complete list, as there is also behind-the-scenes work involved with running a managed service, but it does provide directional insight. Prioritization of this list is continuously evaluated based on product feedback.


## Inner loop performance
Providing a fast, iterative development experience is at the heart of VSCE. We aspire to make the inner loop performance and workflow for VSCE as close to local development as possible.
 
## Improve experience for project references
It is currently not straightforward to successfully F5/debug projects that have VS project-to-project references. We want to streamline this experience for common VS solution structure patterns.
 
## Azure portal experience
Provide an experience for creating, sharing, and managing Connected Environments in the [Azure portal](https://portal.azure.com).
 
## Custom Virtual Network support
The ability to place a Connected Environment, at the time of creation, into an existing Virtual Network. Two key scenarios: 1) Containers running in the Kubernetes cluster need to access Azure services, like SQL and Redis, that are provisioned in an existing VNet. 2) Lock down VSCE endpoints so that they are only accessible from inside the VNet.
 
## Connected Environment size and customization
Provide a way to specify Kubernetes cluster size to best fit budget and workload requirements. We are also considering support for connecting VSCE to an existing AKS instance for more flexibility. 

## Enable non-http protocols
Loosen requirements on service-to-service communication to allow raw TCP, websockets, etc.

## Java debugging
Support a Kubernetes debugging experience for Java containers, similar to current support for .NET Core and Node.js code.
 
## Expand Azure regions
VSCE is currently available in `eastus` and `westeurope`. More regions will be added based on usage patterns.
 
## Publish to AKS from Visual Studio
Provide a familiar experience for publishing a project to AKS via the Visual Studio publish wizard, as defined by the Dockerfile and Helm chart assets in the project. A related scenario under consideration is publishing a solution (of multiple projects).
