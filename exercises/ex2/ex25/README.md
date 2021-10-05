# Exercise 2.5 - Simulate the REST API

The simulation feature allows you to test the integration flow or parts of the flow steps even before you deploy the integration flow. You can run the simulation either in edit or display mode.

## Exercise steps

Run through the following steps, [see also video below](/exercises/ex2/ex25#Demo).
1. In the integration flow model, click on the connection between the *Start* event and the *first Groovy* script, and select the button *Simulation Start Point* from the quick menu
2. Click on the connection right after the *Message Mapping* step, and select the button *Simulation End Point* from the quick menu
3. Click on the *Simulation Start Point*, and upload the zip sample file **SampleRequest.zip** from the **Simulation** folder of the beforehand downloaded material. The zip file contains a sample header file defining the HTTP URL, the HTTP query, and the HTTP path
4. During simulation, no external calls are carried out. So, we need to provide a sample response mocking the Request Reply receiver. Click on the *SOAP connection*, and select the button *Add Simulation Response* from the quick menu
5. In the upcoming dialog, upload the sample response XML file **SampleResponseFromSOAPService.xml**
6. Now, all is set to run the simulation. Select button *Run Simulation* from the editor tool bar
7. Once, the simulation has been successfully completed, you can click on the envelopes in between each step
8. If you select the envelope right after the *Request Reply* step, you should see the values of the properties participantId, month, resource, and service. If you switch to the *Body*, you see the response of the mocked SOAP service call in XML format
9. If you select the envelope at the *Simulation End Point*, you see the mapped message in JSON format

## Demo

The video below shows you how to simulate your integration flow. Best is to run the video by selecting **Open link in new tab** so that you can easily return to this page for further proceeding.

[![Simulate integration flow video](/exercises/ex2/images/CI_SimulateIntegrationFlow_Thumbnail.png)](https://video.sap.com/media/t/1_y47s5qie)

## Summary

At the end of this exercise, you should have successfully carried out a simulation run to ensure that your integration flow runs properly.

Finally, we need to deploy the REST API. Continue to - [Exercise 2.6](/exercises/ex2/ex26)
