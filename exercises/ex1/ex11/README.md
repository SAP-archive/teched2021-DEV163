# Exercise 1.1 - Create a re-usable message mapping

In the following, you will create a new message mapping to map employee birthday data from XML to JSON structure. This message mapping will be a re-usable integration artifact which can be referenced to in multiple integration flows within your integration package.

## Exercise steps

Run through the following steps, [see also video below](#Demo).
1. Within the Cloud Integration Web UI, switch to the *Design* area
2. In the Design area, create a new package with a unique name, e.g., **Teched 2021 Exercise XX** with **XX** the participant number assigned to you
3. In the package, switch to *Edit* mode
4. To create a new message mapping, select menu *Add --> Message Mapping*
5. In the upcoming dialog, enter name **MapToJSON_XX** with **XX** the participant number assigned to you, then click on *OK*
6. The mapping should show up as re-usable artifact of type *Message Mapping* in your integration package. Select the message mapping
7. In the message mapping editor, switch to *Edit* mode
8. First, add a source message to your mapping. Click on the *Add source message* link
9. In the upcoming dialog, select *Upload from File System*
10. Navigate to the folder **Integration Artifacts** of the beforehand downloaded tutorial material, and select the WSDL file **Tutorial_EmployeeDetails.wsdl**, then click on *Open*
11. Next, add a target message. Click on the *Add target message* link
12. Same like before, upload your file. This time, select the Swagger file **swagger_person.json**, then click on *Open*
13. You are guided through the upload of the Swagger file as follows
    1. In the upcoming dialog, select API **/person/findByMonth**
    1. On the next screen, select the HTTP method **GET**
    1. On the next screen, select **RESPONSE**
    1. On the next screen, select the HTTP status code **200**
14. Next, map the source to the target structure as follows via drag&drop
    1. Map the source node **employee** to the target node **GET_Response_200**
    2. Map the source field **person_id** to the target field **id**
    3. Map the source field **date_of_birth** to the target field **dob**
15. When done, click on *Save*

## Demo

The video shows you all the steps described above. Best is to run the video by selecting **Open link in new tab** so that you can easily return to this page for further proceeding.

[![Create mapping video](/exercises/ex1/images/CI_CreateMapping_Thumbnail.png)](https://video.sap.com/media/t/1_idr6d80k)

## Summary

At the end of this exercise, you should have defined a new message mapping.

Continue to - [Exercise 1.2](/exercises/ex1/ex12)
