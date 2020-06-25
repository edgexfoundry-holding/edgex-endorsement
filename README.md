# EdgeX Endorsement

## Introduction

Code, tools, and documentation for validating and endorsing device profiles written by third parties. At a high level you'll need to complete five steps to be eligble for the EdgeX Endorsement Program which will ensure that data provided meets all required components. 

1) Deploy EdgeX using one of the provided cloud templates. Alternatively, you can leverage the latest released compose-file provided here: This ensures a vanilla version of EdgeX is being used without modification to ensure the highest compabitibilty.
2) Compose and deploy your device profile using the Device Profile Modeling tool provided [here](https://www.edgexfoundry.org/tbd). This will ensure the profile is validated and has all required components.
3) Run your device locally, configured to point at the cloud instance of the deployed EdgeX to send data.
4) Once deployed, Run the verification script provided to ensure that core-data has been correctly populated with the data that was sent in the previous step.
5) Submit your device profile along with sample data to EdgeX for approval [here](https://www.edgexfoundry.org/tbd).



## 1) Deploy EdgeX

If you want to see how all of EdgeX works - you can leverage your own Azure account and deploy EdgeX to the cloud. This template leverages Azure Container Instances and will deploy a single group called "edgex-example" with 12 services deployed with 2.4 vCPUs allocated (0.2 vCPUs per service) and 6GB of RAM allocated (0.5 GB per service) with an estimated cost of $0.14904 / hour or $3.57696 / day. 

1 container groups * 3600 seconds * 2.4 vCPU * $0.0000135 per vCPU-s  = ~$0.11664

1 container groups * 3600 seconds * 6 GB * $0.0000015 per GB-s  = $0.0324

memory($0.0324) + cpu($0.11664) = $0.14904 / hour
= $3.57696 / day

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fedgexfoundry-holding%2Fedgex-endorsement%2Fmaster%2Ftemplates%2Fazure%2Fazuredeploy.json).




