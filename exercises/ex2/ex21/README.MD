# Exercise 2.1 - Create the REST API skeleton

In this step, you will create a new REST API and add all required integration flow steps using the integration flow proposal capability.

## Exercise steps

Run through the following steps.
1. In your integration package, switch to the *Edit* mode, and select the *REST API* entry from the *Add* menu
2. In the upcoming dialog, enter name **EmployeeBirthdayRESTAPI_XX** with **XX** the participant number assigned to you, then click on *OK*
3. You will see the newly created REST API in the list of the artifacts. Select the REST API to enter the integration flow editor
4. As you can see, an integration flow has been created based on the REST API template. The integration flow consists of a main process with an HTTP sender adapter, and a subprocess where the actual message orchestration needs to be maintained
5. Switch to *Edit* mode, and rearrange the subprocess as follows
   1. Enlarge the subprocess pool so that you have enough space to add 5 further steps
   2. Move the existing *Content Modifier* step to the very end right before the End event
6. Add the following flow steps between the *Start* event and the existing *Content Modifier* step using the quick menu buttons. You get flow steps proposed based on statistical information, otherwise you have the option to search for flow step types if not listed as proposed step. This helps you accelerating the creation of the flow step skeleton. **See also video below**
   1. Add a *Groovy Script* step
   2. Add a *Content Modifier* step
   3. Add a *Request Reply* step
   4. Add a new *Receiver*
   5. Connect the *Request Reply* step with the *Receiver*, here select the *SOAP 1.x* adapter type
   6. Add another *Groovy Script* step
   7. Add a *Message Mapping* step
7. Finally, save your changes

## Demo

The video below shows you how to use the flow step proposal to create the integration flow model. Best is to run the video by selecting **Open link in new tab** so that you can easily return to this page for further proceeding.

[![Deploy mapping video](/exercises/ex2/images/CI_FlowStepProposals_Thumbnail.png)](https://video.sap.com/media/t/1_g11b4yvx)

## Summary

At the end of this exercise, your REST API flow step model has been created.

Next, the flow steps need to be configured. Continue to - [Exercise 2.2](/exercises/ex2/ex22)
