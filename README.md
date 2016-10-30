# Sample code for MS Tech Summit 2016 Japan

## ASP.NET Core Sample app

* Referecnce: [Exploring ASP.NET Core with Docker in both Linux and Windows Containers](http://www.hanselman.com/blog/ExploringASPNETCoreWithDockerInBothLinuxAndWindowsContainers.aspx)

* Two Dockerfiles
  * Switch file to build Docker image
  * Dockerfile.linux for Linux
  * Dockerfile.nano for Windows Nano Server

## DC/OS

* ARM Template for DC/OS
  * As of today, I reccomend to use Azure PowerShell to deploy this Template instead of Azure xplat CLI. Reference: [Default value being ignored when deploying with parameter file](https://github.com/Azure/azure-xplat-cli/issues/3225)
  * set your SSH public key to the parameter
* Deploy Sample app to DC/OS
  * Use this [congiguration](https://github.com/ToruMakabe/TechSummit2016/blob/master/DCOS/Marathon/sampleaspdnc.json)
  * Change labels.HAPROXY_0_VHOST value to your public DNS name of Azure LB