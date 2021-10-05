# Exercise 3.2 - Test the API proxy

Let's test the beforehand created API proxy. For this, we can use the inbuilt test capability.

## Exercise steps

Run through the following steps, [see also video below](#Demo).
1. Switch to the *Test* area
2. In the *API Test Console*, search for your API by entering your participant number **XX**
3. Select your API **EmployeeBirthdayRESTAPI_XX_1_0** with **XX** the participant number assigned to you
4. Change the URL path as follows: replace the wildcard __*__ with the service **hr** and the resource **employee**, i.e. enter **hr/employee**. The path should be **/10/XX/hr/employee** with **XX** the participant number assigned to you
5. Let's run the GET request by selecting the *Send* button on the bottom right
6. As response you should see the full list of employee IDs including their birthday in JSON format
7. Let's run a second time, this time we like to fetch the data for employees born in a particular month. So Click on the *Url Params* button, and enter parameter name **month** and any value between **01** and **12**, then click on *Send* again
8. As response you should see the list of employees born in the chosen month, in the video below we have chosen March and hence get one single entry displayed

## Demo

The video below shows the exercise steps as described above. Best is to run the video by selecting **Open link in new tab** so that you can easily return to this page for further proceeding.

[![Test API video](/exercises/ex3/images/APIM_RunAPI_Thumbnail.png)](https://video.sap.com/media/t/1_kdmczl3p)

## Summary

At the end of this exercise, you should have successfully run the API proxy of version 1.0.

Continue to - [Exercise 3.3](/exercises/ex3/ex33)
