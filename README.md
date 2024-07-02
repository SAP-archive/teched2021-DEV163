[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2021-DEV163)](https://api.reuse.software/info/github.com/SAP-samples/teched2021-DEV163)
[![Not Maintained](https://img.shields.io/badge/Maintenance%20Level-Not%20Maintained-yellow.svg)](https://gist.github.com/cheerfulstoic/d107229326a01ff0f333a1d3476e068d)

 
# DEV163 - Get Hands-On Experience with SAP Integration Suite

## Description

Get your hands dirty learning the latest and greatest of SAP Integration Suite, SAP's hybrid integration platform offering for enterprise-wide integration needs.  

## Overview

This session introduces you to new features of SAP Integration Suite that have been recently shipped. Here, we focus on two SAP Integration Suite capabilities namely Cloud Integration and API Management. When running through the exercises, you will touch a couple of new features such as:
- Low code API development
- Script collection
- Message mapping as reusable artifact
- Flow step recommendations
- Integration flow simulation
- JSON message mapping based on Swagger file
- Show deployment status in designer
- Monitoring enhancements: search based on payload data
- Discover integration flows in API Management designer
- Versioning of APIs

### Scenario setup

You would like to send birthday greetings for all employees which celebrate their birthday in the current month. For this, you will create a simple REST API to query the employee birthday data for a particular month. Within the REST API implementation, you will call a SOAP service provided by us mocking an HR system. The data is expected to be provided in JSON format, so a transformation from XML to JSON is required. The REST API should be accessible from your centralized API catalog. Furthermore, you need to add a policy for traffic management purposes.
So, in a nutshell, the following steps need to be performed:
- In Cloud Integration, you will create a message mapping and a script collection as re-usable artifacts that are required within your REST API
- In Cloud Integration, you will create, implement and deploy a new REST API providing the employee birthday data
- In API Management, you will create an API proxy based on the beforehand created REST API
- In API Management, you will add a traffic policy to a new version of the API proxy

## Requirements

There are no prior requirements to this exercise. You can perform this even if you do not have any experience with integration solutions. However, you will be able to derive a lot of value from this session if you have some knowledge on what SAP Integration Suite is all about and how it helps with enterprise-wide integration needs.

Here are two missions that can help you getting started with SAP Integration Suite:

- [Get Started with Integration Suite - Cloud Integration](https://discovery-center.cloud.sap/protected/index.html#/missiondetail/3258/3327/)
- [Get Started with Integration Suite - API Management](https://discovery-center.cloud.sap/protected/index.html#/missiondetail/3062/3072/)


## Exercises

In the following, the complete list of exercise steps are listed. Run through them in the given order. You can use this section as an index or table of contents. Use the breadcrumb navigation on top of the pages to go back to the Table of Contents.

### Prepare
- [Getting Started](exercises/ex0/)

### [Exercise 1 - Create Re-usable Artifacts](exercises/ex1/)
- [Create a re-usable message mapping](exercises/ex1/ex11)
- [Optional - Test your message mapping](exercises/ex1/ex12)
- [Deploy your message mapping](exercises/ex1/ex13)
- [Import and deploy a script collection](exercises/ex1/ex14)

### [Exercise 2 - Create a REST API](exercises/ex2/)
- [Create a new REST API](exercises/ex2/ex21)
- [Add references to the REST API](exercises/ex2/ex22)
- [Maintain the REST API end point](exercises/ex2/ex23)
- [Maintain the REST API flow steps](exercises/ex2/ex24)
- [Simulate the newly created REST API](exercises/ex2/ex25)
- [Deploy your REST API](exercises/ex2/ex26)

### [Exercise 3 - Create an API Proxy](exercises/ex3/)
- [Create an API proxy](exercises/ex3/ex31)
- [Test your API proxy](exercises/ex3/ex32)
- [Create a new API version & add a policy](exercises/ex3/ex33)
- [Test your new API proxy version](exercises/ex3/ex34)
- [Optional - Monitor your messages](exercises/ex3/ex35)



## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2021 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
