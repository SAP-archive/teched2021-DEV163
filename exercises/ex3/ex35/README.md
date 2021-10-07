# Exercise 3.5 (Optional) - Monitor the message exchange

Monitoring has been enhanced so that you can now display the custom header properties in the message processing log (MPL) monitor. Furthermore, you can use all MPL header attributes in the search filter.

## Exercise steps

Run through the following steps.
1. Navigate to the SAP Integration Suite landing page by selecting the Integration Suite link in the top bar
2. On the landing page, select the Cloud Integration tile to open the Cloud Integration Web UI
3. Switch to the Operations view.
4. In the Monitor, click on the All REST APIs tile. If the tile does not exist, add it by clicking on the Plus sign tile below the Monitor Message Processing section
5. In the Monitor Message Processing, narrow down the list of log entries by using the filter. Click on the Use More Fields button
6. Here, you have different filter options based on the MPL and custom header properties.
   1. In the Application Message Type filter, select person_XX with XX the number assigned to you
   2. In the Custom Header enter month=## with ## the month that you have used previously when testing the APIs, e.g., 03. Then click enter
8. This will display you your logs. If you scroll down, you can see that the custom header properties are displayed in the Properties section of the log

![Configure REST API](/exercises/ex3/images/CI_Moni.png)


## Summary

At the end of this exercise, you have learned about the search and filter capabilities in the message monitoring.

Congratulations, this concludes the overall tutorial. Navigate back to - [Exercise overview page](/README.md)
