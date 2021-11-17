# Exercise 2.4 - Maintain the REST API flow steps

In this exercise, we will maintain all flow steps of the subprocess of your API.

## Exercise steps

Run through the following steps to configure the flow steps of the subprocess from left to right.

### First Groovy script

Let's start with the first Groovy script. The first Groovy script reads the URL path as well as the GET parameter if provided.
1. Select the first Groovy script, and switch to the *Processing* tab
2. Click on *Select*
3. In the upcoming dialog, switch to the *Referenced Resources* tab
4. Select the entry **ReadUrlPath**, then click on *OK*
5. As *Script Function*, maintain **extractUrlPathAndQuery**

### First Content Modifier

In the subsequent Content Modifier step, we need to define the request body for the Request Reply lookup.
1. Select the Content Modifier step
2. Switch to the *Exchange Property* tab, and create a new property of name **participantId**, type **Constant**, and value **XX** whereas replace **XX** with the participant number assigned to you
3. Switch to the *Message Body* tab, and maintain the body of type *Expression* as follows:
```
<?xml version='1.0' encoding='UTF-8'?>
<ns0:employeeRequest xmlns:ns0="http://tutorial.sap.com" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
<id>${property.id}</id>
<operation>${property.operation}</operation>
<month>${property.month}</month>
</ns0:employeeRequest>
```

### Request Reply step

For the Request Reply step, we need to maintain address URL and credentials.
1. Select the *SOAP* connection, and switch to the *Connection* tab
2. In the *Address* field, maintain **{{address}}** to create an externalized parameter with name address
3. Select *Basic Authentication* from the drop down menu
4. In the *Credential Name* field, maintain **{{credentials}}** to create an externalized parameter with name credentials

**Note**: The values of the externalized parameters will be maintained when configuring the REST API.

### Second Groovy script

We need another Groovy script to set the custom header. This is required for monitoring purposes.
1. Select the second Groovy script, and switch to the *Processing* tab
2. Click on *Select*
3. In the upcoming dialog, switch to the *Referenced Resources* tab
4. Select the entry **MPLCustomHeader**, then click on *OK*
5. As *Script Function*, maintain **setCustomHeader**

### Mapping

The response from the SOAP request should be mapped from XML to JSON format.
1. Select the Message Mapping step, and switch to the *Processing* tab
2. Click on *Select*
3. In the upcoming dialog, switch to the *Referenced Resources* tab
4. Select the entry **MapToJSON_XX** with **XX** the participant number assigned to you, then click on *OK*

### Second Content Modifier

Finally, we need to define the proper content type.
1. Select the Content Modifier step
2. Switch to the *Message Header* tab, and create a new header of name **content-type**, type **Constant**, and value **application/json**
3. When done, save your changes

**Note**: After saving the integration flow model, you will see an error on the SOAP connection. This is due to the fact that the externalized address parameter is still empty. No worries, you can continue with the next exercise, the error will be gone once we configure the parameter.

## Summary

At the end of this exercise, you should have configured all flow steps of your REST API.

Continue to - [Exercise 2.5](/exercises/ex2/ex25)
