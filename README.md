# EdgeX Endorsement

## Introduction

Code, tools, and documentation for validating and endorsing device profiles written by third parties.


## Quick Start

If you want to see how all of EdgeX works - you can leverage your own Azure account and deploy EdgeX to the cloud. This template leverages Azure Container Instances and will deploy a single group called "edgex-example" with 12 services deployed with 2.4 vCPUs allocated (0.2 vCPUs per service) and 6GB of RAM allocated (0.5 GB per service) with an estimated cost of $0.14904 / hour or $3.57696 / day. 

1 container groups * 3600 seconds * 2.4 vCPU * $0.0000135 per vCPU-s  = ~$0.11664

1 container groups * 3600 seconds * 6 GB * $0.0000015 per GB-s  = $0.0324

memory($0.0324) + cpu($0.11664) = $0.14904 / hour
= $3.57696 / day

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fedgexfoundry-holding%2Fedgex-endorsement%2Fmaster%2Ftemplates%2Fazure%2Fazuredeploy.json).


