# Exercise 2.6 - Deploy the REST API

In the last exercise of the second part of the tutorial, we need to deploy the beforehand created and maintained REST API. Before we can deploy the REST API, we need to configure the externalized parameters.

## Exercise steps

Run through the following steps.

### Fetch URL of mocked service
First let's configure the address of the SOAP service that is called within the REST API. We have actually defined and deployed an integration flow on the Cloud Integration tenant mocking the SOAP service
1. In the Cloud Integration Web UI, switch to the *Operations* view by selecting the *Monitoring* entry in the navigation pane
2. In the monitor, select the *All* tile below the *Manage Integration Content* section
4. In the *Manage Integration Content* view, search for **Employee Birthday SOAP Service - Solution**, and select the integration flow found
5. On the *Endpoints* tab, copy the entry point URL to the clipboard

### Configure the externalized parameters
1. Switch back to the *Design* area, and open your integration package
2. In your integration package, select entry *Configure* from the *Actions* quick menu of your REST API, see picture below
3. In the upcoming dialog, paste the URL from the clipboard into the *Address* parameter
4. We have already deployed a credential with name **OWN** to authenticate towards the SOAP service. So, enter the value **OWN** into the *Credential Name* parameter
5. Click on *Save*
6. Once saved, click on *Deploy*, and confirm the upcoming dialog
7. Optionally, you can switch to the *Operations* view again, and check the status of your deployed REST API in the *Manage Integration Content* monitor

<br>![Deploy REST API](/exercises/ex2/images/CI_Configure&DeployRESTAPI.png)

## Summary

At the end of the second part of the tutorial, you should have a running REST API on the Cloud Integration tenant to fetch employee birthday data.

In the last part of the tutorial, we will consume this REST API in API Management. Continue to - [Exercise 3](/exercises/ex3)
