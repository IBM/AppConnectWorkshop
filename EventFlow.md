# Building a Event Driven Flow with Http Response and Cloudant 

As described in the main [ReadME](https://github.com/pmmistry/AppConnectWorkshop#event-driven-flows),Event driven flows enable you to identify an event that can occur in your first application (the source application), and actions that can be performed in one or more target applications. 

In today's workshop we will configure a simple Event driven flow that uses a Scheduler node to kick off a response from an Http response node (the source application) to send data into a Cloudant database (the target application)

## Prerequisites
- [Create IBM Cloud Account](https://github.com/pmmistry/AppConnectWorkshop#prerequisites)
- [Create App Connect Service](https://github.com/pmmistry/AppConnectWorkshop#prerequisites)
- [Create Cloudant Database](https://github.com/pmmistry/AppConnectWorkshop#prerequisites)
- [Create Event Stream Service(Optional)](https://github.com/pmmistry/AppConnectWorkshop#setting-up-event-stream-optional)

## Workshop

### Step 1 
Start off by launching your App Connect Service. Omce you have launched your service click on `Create an event-driven flow`
![](./images/img11.png)

### Step 2
To add applications to your flow, Click on '+' and select applications that you want to add to your flow. We are first going to start of with the `Scheduler` tool. To add this to your flow, `+ > Toolbox > Scheduler` 
![](./images/img12.png)

> Also give your flow a name. I called mine `Http Response Flow` 

### Step 3 
Configure the scheduler component according to your preferences. Here I am creating a flow that sends http response for an API  every one minute. I have also set it to run when the flow is first switched on. 
![](./images/img13.png)

### Step 4 
To add the next node to the flow, click on '+'. Here, we are adding Http Response node so that we will be able to send an API response at scheduled time. To do this, `+ -> Applications -> HTTP -> Invoke method`. Once you have that set click `Connect`
![](./images/img14.png)

We will be working with the following API : `https://reqres.in/api/users/1`

Add this API to the `Secure Gateway Protocol` and click `Connect`: 
![](./images/img15.png)

You will then need to set the Invoke Method details. 
 - Set HTTP method to `GET`
 - Set URL to API url : `https://reqres.in/api/users/1`

![](./images/img16.png)

You should now have you API method all set up. You can actually test your API by clicking on the `Try this action button` : 

![](./images/img17.png)
If you click on `View details` you should see the details of your actions : 

![](./images/img18.png)

