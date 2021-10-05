# Exercise 3.3 - Create an API version and add a policy

In this exercise of the tutorial, we will cover the topic of API versioning. Versioning allows the creation and management of multiple releases of an API. You can version an API proxy when you want to improve, upgrade, or customize the functional behavior provided by a currently existing API proxy. In our case, we will create a new version of the beforehand created API proxy, and add a policy to the same.

## Exercise steps

Run through the following steps, [see also video below](#Demo).
1. Switch back to the *Develop* area
2. For your beforehand created API proxy **EmployeeBirthdayRESTAPI_XX_1_0**, select *New Version* from the *Action* menu
3. In the upcoming dialog, maintain version **1.1**. You will notice that the base path is automatically updated to **/11/tutorial/XX/*** and the name is changed to **EmployeeBirthdayRESTAPI_XX_1_1**. Then, click the *Create* button
4. In the API editor, select *Policies* from the top right
5. In the Policy editor, expand the *ProxyEndpoint*, and select the *PreFlow*
6. In the Policies navigation pane, below the *Traffic Management Policies*, add the *Quota* policy by clicking on the *Plus* sign
7. In the upcoming dialog, enter a policy name, e.g., **myQuota**, and click the *Add* button
8. Keep the allow count to **2**, and the interval to **1**, i.e., only two calls per minute are allowed
9. Click on *Update* on top
10. Finally, save and deploy the new version of the API proxy

## Demo

The video below shows the exercise steps as described above. Best is to run the video by selecting **Open link in new tab** so that you can easily return to this page for further proceeding.

[![Create API version video](/exercises/ex3/images/APIM_CreateNewAPIVersion_Thumbnail.png)](https://video.sap.com/media/t/1_5wg8sjno)

## Summary

At the end of this exercise, you should have created a new API proxy version 1.1 and added a policy.

Continue to - [Exercise 3.4](/exercises/ex3/ex34)
