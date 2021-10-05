# Exercise 2.3 - Maintain the REST API end point

Next, we will maintain the end point of the REST API.

## Exercise steps

Run through the following steps.
1. In the integration flow editor, select the *HTTP connection* of the main process
2. Switch to the *Connection* tab
3. Maintain the Address as **/tutorial/restapi/XX/*** with **XX** the participant number assigned to you

<br>![Add references](/exercises/ex2/images/CI_EndPoint.png)

**Note**: Since we use a wildcard in the endpoint of the REST API, we can call the REST API passing different values for service, resource and id whereas id is optional. Furthermore, we can use GET parameters to define a filter. Sample URL paths may look as follows:
- **/tutorial/restapi/XX/hr/employee/PER-5044** to fetch date of birthday for a particular employee with id **PER-5044**
- or **/tutorial/restapi/XX/hr/employee?month=03** to fetch all employees which were born in **March**

## Summary

At the end of this exercise, you should have maintained a unique end point of your REST API.

Continue to - [Exercise 2.4](/exercises/ex2/ex24)
