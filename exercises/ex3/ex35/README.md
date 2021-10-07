# Exercise 3.5 - Monitor the message exchange

Monitoring has been enhanced so that you can now display the custom header properties in the message processing log (MPL) monitor. Furthermore, you can use all MPL header attributes in the search filter.

## Exercise steps

Run through the following steps.
1. Navigate to the SAP Integration Suite landing page by selecting the Integration Suite link in the top bar
2. On the landing page, select the Cloud Integration tile to open the Cloud Integration Web UI
3. Switch to the Operations view. Then, click on the Monitoring Message Processing tile
4. Narrow down the list of log entries by using the filter. Click on the Use More Fields button
5. As you can see, you have different filter options based on the MPL and custom header properties. Furthermore, the custom header properties are displayed in the Properties section of the log


### Configure the externalized parameters & deploy
1. Switch back to the *Design* area, and open your integration package
2. In your integration package, select entry *Configure* from the *Actions* quick menu of your REST API

![Configure REST API](/exercises/ex2/images/CI_Configure&DeployRESTAPI.png)

3. In the upcoming dialog, paste the URL from the clipboard into the *Address* parameter
4. We have already deployed a credential with name **OWN** to authenticate towards the SOAP service. So, enter the value **OWN** into the *Credential Name* parameter
5. Click on *Save*
6. Once saved, click on *Deploy*, and confirm the upcoming dialog
7. Select the REST API to enter the integration flow editor
8. Once the REST API has been successfully started, you can see its deployment status on the very top next to the name of the integration flow
9. Furthermore, in the *Properties* section of the integration flow, switch to the *Deployment Status* tab to get more status information displayed

![Deployment status REST API](/exercises/ex2/images/CI_DeploymentStatus.png)

10. Optionally, from here you can actually navigate to the *Manage Integration Content* monitor

## Summary

At the end of the second part of the tutorial, you should have a running REST API on the Cloud Integration tenant to fetch employee birthday data.

In the last part of the tutorial, we will consume this REST API in API Management. Continue to - [Exercise 3](/exercises/ex3)
