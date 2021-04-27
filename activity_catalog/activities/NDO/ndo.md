# Network Dev Ops Agent - NDO

Network Dev Ops Agent is an run time environment that allows to manage execution remotely via a REST api.  NDO Agents are ideal for deployment in a production environment as they provide multiple language support as well as the security capability of only executing signed/certified assets.


# Installation

Installation is support on Ubuntu and REHL (refer to user guide for currently supported versions).
 
## Summary of steps  


- Download the nda_linux_x.x.x.run from CSC
- Edit /etc/opt/spirent/nda/agent.conf
	- number of processes (each requires a NDO license)
	- License server
	- password authorization file (This file will need to be created)
- start NDO
	- sudo /etc/init.d/nda start
- Monitor status
	- sudo /etc/init.d/nda status
- Stop NDO
	- sudo /etc/init.d/nda stop

## Test NDO is working - This is also the NDO api guide
- Browse to https://your.ndo.instance.com:8080/api/doc


## Using NDO - brief api overview
Auth - Setup and username and passwords (these are stored in the authorization file
AUTH	- Authentication and new user creation
Capabilities - query NDO agent capabilities
Executions - start and monitor test executions
Testcase - Returns the list of test cases including test case
Parameters - Provides parameter file details


#NDO Reference


