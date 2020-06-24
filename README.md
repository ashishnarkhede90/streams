<a style="float: right;" href="https://githubsfdeploy.herokuapp.com?owner=bigassforce&amp;repo=streams&amp;ref=master">
    <img alt="Deploy to Salesforce" src="https://github.com/bigassforce/streams/wiki/48-deploy-to-salesforce.png">
</a>

Streams are durable event pipelines that give your code increased limits and the ability to recover from any error.

<br/>

## Getting Started

- Install the [Streams Package](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t7F000003irjN)

<br/>

## Simplest Possible Thing

<img align="right" src="https://github.com/bigassforce/streams/wiki/48-simplest-thing.png" align="right" />

1. From the **Streams** app, go to the **Services** tab.
2. Click the  **Log** service and view its detail page.
3. Click **Enqueue** then check your email.

See the log email? Here's what happened:

First your event was stored in a record, then the Log service processed it in a try-catch block with a savepoint.

Although the service just sends an email, the key takeaway is this: everything
<br/>is processed safely in an async context with increased limits, without writing code.

![](https://github.com/bigassforce/streams/wiki/48-simplest-thing-event.png)

<br/>

## Next Steps
Try the <a href="https://github.com/bigassforce/streams/wiki/Pipes-Tutorial">Pipes Tutorial</a>. This assembles many services in an arrangement known as a pipe.
<br />Below are the three core concepts, each one can be explored via its own tab in the app:

- [Services](https://github.com/bigassforce/streams/wiki/Standard-Services) - any class that implements `Callable`
- [Events](https://github.com/bigassforce/streams/wiki/Events) - a piece of data represented as JSON
- [Pipes](https://github.com/bigassforce/streams/wiki/Pipes) - an arrangement of services in order

For a more in-depth look, see the <a href="https://github.com/bigassforce/streams">source code</a> of the standard services.

<br/>


## Features
- All config aspects support versions with effective dating
- Audit past and present events - understand which logic ran and when
- Collaborate using components that all business stakeholders can understand

##### Admins
- Isolate clicks from code by using a service as a container
- Configure pipes, steps and services with metadata or change sets
- Integrate to and from flows, processes and workflow rules using events
- Recover from processing failures and resolve data issues without a developer

##### Developers
- Graceful error handling using stored events to debug or reproduce
- Maximise performance with automatic bulkification of DML side effects
- Create easily tested code using components that adhere to an interface
- Insert complex SObject hierarchies with relationships ordered automatically

##### Consultants
- Integrate using HTTP / SMTP / SQL adapters
- Control scope with clear areas of responsibility
- Reduce maintenance costs with simpler code/data handover
- Lower risk for proof of concepts without early commitment to architecture
- Loose coupling between departments using JSON events instead of compiled dependencies

<img src="https://bigass.secure.force.com/pixel?url=https://github.com/bigassforce/streams/wiki/Home" />
