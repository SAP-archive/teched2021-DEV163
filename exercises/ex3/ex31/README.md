# Exercise 3.1 - Create an API proxy

In this exercise, you will create a new API proxy based on the previously deployed RESTful API.

## Exercise steps

Run through the following steps, [see also video below](#Demo).
1. In the *API Portal*, switch to the *Develop* area
2. On the *APIs* tab, click on the button *Create*
3. In the upcoming dialog, select the API provider *demo_discover* from the drop down list, and click the *Discover* button
4. Search for your participant number assigned to you
5. From the list of deployed APIs, select your API **EmployeeBirthdayRESTAPI_XX** with your participant number **XX**, then click on the *Next* button
6. On the next screen, you can choose from different authentication types to access the API metadata
   1. Here, we select the authentication type *OAuth2ClientCredentials* from the drop down menu
   2. Then, maintain *Client ID*, *Client Secret*, and *Token URL*. You find the required information in the **serviceKey_Runtime.txt** file that you have downloaded before.
   3. Then click the *Done* button.
7. On the next screen, maintain the API details.
   1. You can keep the proposed *Name* and *Title*
   2. Change the *API Base Path* to **/tutorial/XX/*** with **XX** your participant number
   3. Maintain Version **1.0**. You will notice that when entering a version, the API base path and the name are automatically adapted accordingly: the API base path should be automatically changed to **/10/tutorial/XX/***, the name is automatically changed to **EmployeeBirthdayRESTAPI_XX_1_0**
8. When done click the *Create* button
9. For now, we won't maintain any policies. So click the *Save* button
10. Finally, deploy the API proxy

## Demo

The video below shows the exercise steps as described above. Best is to run the video by selecting **Open link in new tab** so that you can easily return to this page for further proceeding.

[![Create API video](/exercises/ex3/images/APIM_CreateAPIProxy_Thumbnail.png)](https://sapvideoa35699dc5.hana.ondemand.com/?entry_id=1_80z9vlnx)

## Summary

At the end of this exercise, you should have created and deployed an API proxy.

Continue to - [Exercise 3.2](/exercises/ex3/ex32)
