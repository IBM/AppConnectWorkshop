# Building Integrations with App Connect 

[IBM® App Connect](https://www.ibm.com/cloud/app-connect) instantly connects applications and data from existing systems and modern technologies across all environments. You can use App Connect to create event-driven flows or flows for APIs. 

### Event Driven Flows: 
In an event-driven flow, you identify an event that can occur in your first application (the source application), and actions that can be performed in one or more target applications. The flow links the event to the actions so that, whenever the event occurs in the source application, the action is automatically triggered in the target applications.

For example, you might create a flow so that whenever someone registers as a new attendee with Eventbrite (the event), App Connect automatically retrieves details of the attendee from Salesforce and creates a task in Asana (the actions). 

![](./images/img1.jpg)

### Flows for API:
A flow for an API contains a request, one or more target application actions, and a response. The request uses a model that you define to request the creation, replacement, or retrieval of data objects in your applications. When the request is submitted, each target application performs its action. The flow then returns a response that either confirms that the actions were successful, or returns the data that was requested.

![](./images/img2.jpg)


### In tutorial we will go through: 
- Lab 1 : Creating Event Driven Flow with Http Requests and Cloudant
- Lab 2 : Creating API Flow
- Lab 3 : Working with Templates and Slack 

## Getting Started: 
In this session we will get you started with creating a Lite App Connect Service on IBM Cloud 

### Prerequisites
Register and create an [IBM Cloud Account](https://cloud.ibm.com/login) 

### Setting up App Connect Service 

#### Step 1: 
Let's go to [IBM Cloud Catalog](https://cloud.ibm.com/catalog) and search for App Connect.
![](./images/img3.png)

### Step 2: 
Select `Lite` Plan and give your service a name. Click on the `Create` Button to create your Lite service
![](./images/img4.png)

### Step 3: 
Launch the service by clicking `Launch App Connect`
![](./images/img5.png)



 


