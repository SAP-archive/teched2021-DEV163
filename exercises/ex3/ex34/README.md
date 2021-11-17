# Exercise 3.4 - Test the new API proxy version

As a last step within the tutorial, we test the beforehand created new API proxy version. like before, we can use the inbuilt test capability.

## Exercise steps

Run through the following steps, [see also video below](#Demo).
1. Switch to the *Test* area
2. In the API Test Console, search for your API by entering your participant number **XX**
3. Select your new API version **EmployeeBirthdayRESTAPI_XX_1_1** with **XX** the participant number assigned to you
4. Change the URL path as follows: replace the wildcard __*__ with the service **hr** and the resource **employee**, i.e. enter **hr/employee**. The path should be **/11/XX/hr/employee** with **XX** the participant number assigned to you
5. Click on the *Url Params* button, and enter parameter name **month** and any value between **01** and **12**, then click on *Send*
6. As response you should see the list of employees born in the chosen month, in the video below we have chosen May
7. Repeat the sending twice within the minute. After the overall third call, you should see a fault message indicating that the quota limit has been exceeded

## Demo

The video below shows the exercise steps as described above. Best is to run the video by selecting **Open link in new tab** so that you can easily return to this page for further proceeding.

[![Test API version video](/exercises/ex3/images/APIM_RunNewAPIVersion_Thumbnail.png)](https://sapvideoa35699dc5.hana.ondemand.com/?entry_id=1_blb5k1bl)

## Summary

At the end of this exercise, you should have successfully run the new API proxy version and verified that the policy has been applied.

This more or less concludes the overall tutorial. You may navigate back to - [Exercise overview page](/README.md)

If you however like to know more about the message monitoring filter options, you can continue to the optional exercise - [Exercise 3.5](/exercises/ex3/ex35)
