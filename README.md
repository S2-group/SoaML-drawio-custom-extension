<h1 style="text-align: center;"> SoaML Extension for Diagrams.net </h1>

# About

This extension is a collection of SoaML libraries that enables the user to draw SoaML diagrams within the <a>diagrams.net</a> web application and the <a>draw.io</a> desktop App created by <a>JGraph Ltd</a>. The diagrams in each library are based on the <a href="http://www.omg.org/spec/SoaML/">OMG SoaML specification</a>.

The SoaML extension for diagramas.net was developed as part of my bachelor's thesis at the Vrije Universiteit Amsterdam and is specifically designed to provide students of the <a href="https://studiegids.vu.nl/EN/courses/2022-2023/X_405061#/">Service Oriented Design</a> course taught by <a href="https://research.vu.nl/en/persons/patricia-lago">prof. dr. Patricia Lago</a> as part of the <a href="https://vu.nl/en/education/master/computer-science/curriculum?year=1st-year&specialization=software-engineering-and-green-it">Software Engineering and Green IT</a> track for the Master's in Computer Science at Vrije Universiteit Amsterdam with a lightweight open-source tool to draw SoaML diagrams for their course assignments. However, this extension is also open for use and modification by anyone who is interested in modeling SOA systems using the SoaML notations provided.

This extension provides the user with a colleciton of 5 SoaML libraries, with each library containing the elements for a specific SoaML diagram.

The 5 libraries are:

1. **SoaML-Interface:** For drawing Simple Interface and Service Interface Diagrams.
2. **SoaML-Participant:** For drawing Participant Diagrams.
3. **SoaML-ServiceContract:** For drawing Service Contract Diagrams.
4. **SoaML-ServicesArchitecture:** For drawing Services Architecture Diagrams.
5. **SoaML-Templates:** Examples of the aforementioned diagrams.

These libraries provide the user with the ability to specify services from different points of view, enabling the user to understand how different components provide and use services as well as how they interact with one another within a Services Oriented Architecture (SOA) system in order to to achieve a business goal.

# Table of Contents

- [What is SoaML?](#what-is-soaml)

- [Setting Up the SoaML Extension for Diagrams.net](#setting-up-the-soaml-extension-for-diagramsnet)

- [Drawing SoaML Diagrams in Diagrams.net](#drawing-soaml-diagrams-in-diagramsnet)

  - [What to expect from this tutorial?](#what-to-expect-from-this-tutorial)

  - [Drawing Service Interface Diagrams](#drawing-service-interface-diagrams)

  - [Drawing Participant Diagrams](#drawing-participant-diagrams)

  - [Drawing Service Contract Diagrams](#drawing-service-contract-diagrams)

  - [Drawing Services Architecture Diagrams](#drawing-services-architecture-diagrams)

- [SoaML Templates](#soaml-templates)

# What is SoaML?

Service Oriented Architecture Modeling Language (SoaML) is a tool specified and maintained by the <a href="https://www.omg.org/">Object Management Group (OMG)</a> that enables us to model services through the use of modified Unified Modeling Language (UML) notations. In order to fully understand the purpose of SoaML let us be reminded of what goes on in a Service Oriented Architecture (SOA) System. In SOA systems, participants exist in a community, or a distributed computing environment and they use and provide services in order to achieve a common goal which are usually tied to a business process. Participants can be defined as people, organizations, or different components of a system. A service is defined as a value that is exchanged. In order for participants to provide or use services, they must play the role of a service provider or a service consumer.

SoaML extends the UML profile to enable the specification of services in three possible approaches as described by the OMG SoaML Specification: The Simple Interface Approach, Service Interface Approach, and Service Contract Approach. Additionally, SoaML allows us to model a service network through the use of the Services Architecture diagram in order to describe how each participants collaborate as a community within a SOA system.

# Setting Up the SoaML Extension for Diagrams.net

### **Method 1 (Recommended): Directly importing the libraries package from the Github Repository to diagrams.net:**

**To import the libraries package directly from the Github Repository to diagrams.net simply click on this <a href="https://app.diagrams.net/?splash=0&clibs=Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fgiva16%2Fdrawio-custom-lib%2Fmain%2FSOAML%2520Library%2FSoaML-General.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fgiva16%2Fdrawio-custom-lib%2Fmain%2FSOAML%2520Library%2FSoaML-Interface.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fgiva16%2Fdrawio-custom-lib%2Fmain%2FSOAML%2520Library%2FSoaML-Participant.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fgiva16%2Fdrawio-custom-lib%2Fmain%2FSOAML%2520Library%2FSoaML-ServicesArchitecture.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fgiva16%2Fdrawio-custom-lib%2Fmain%2FSOAML%2520Library%2FSoaML-ServiceContract.xml;Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fgiva16%2Fdrawio-custom-lib%2Fmain%2FSOAML%2520Library%2FSoaML-Templates.xml">link</a>**, this link will directly import the libraries from the github repository to the diagrams.net web application's library manager. The libraries will be stored in the local storage of your web-browser.

<img src="Images/Tutorial Images/Setting Up Library/1.gif">

**To Update the libraries:** Close the libraries in diagrams.net and click on this link again. This will update the libraries in the local storage of your web-browser.

<img src="Images/Tutorial Images/Setting Up Library/2.gif">

**\*Note:** _This method does not allow the user to modify the libraries and templates and is not available for the offline diagrams.net desktop application._

### **Method 2 (Allows User to Modify Libraries and Templates): Downloading the repository and importing the libraries package to diagrams.net/draw.io desktop:**

1. Click on the link download the library package: <button><a href="https://download-directory.github.io?url=https://github.com/giva16/drawio-custom-lib/tree/main/SOAML%20Library" download>Download Library Package</a></button>

2. Extract the zip file to a folder of your choice.

3. Open the <a href="https://app.diagrams.net/">diagrams.net</a> web application or the draw.io desktop App.

4. Create a new blank diagram by clicking "Create New Diagram" > Select "Blank Diagram" > Click "Create".
   <img src="Images/Tutorial Images/Setting Up Library/3.gif">
5. Give your new diagram a name on the top left corner of the editor.
   <img src="Images/Tutorial Images/Setting Up Library/4.gif">

6.1 **To Load the library one by one** Click on "File" > "Open Library From" > "Device..." > Open the "SOAML Library" folder that you extracted in step 2 > Select the XML file of the library you want to load > Click "Open".

6.2 **To Load multiple or all libraries at once** Open the "SOAML Library" folder that you extracted in step 2 > Select all the XML files of the libraries you want to load > Drag and drop the selected files into the editor.
<img src="Images/Tutorial Images/Setting Up Library/5.gif">

7. You can now view all the SoaML elements in the library panel on the left side of the editor and you have everything you need to start drawing SoaML diagrams.

   <img src="Images/Tutorial Images/Setting Up Library/6.png">

   **Happy Drawing!**

# Drawing SoaML Diagrams in diagrams.net

## What to expect from this Tutorial?

This tutorial will guide the user on how to draw SoaML diagrams using the SoaML libraries provided by this extension. The tutorials will guide the user on how to draw the Service Interface Diagram, Participant Diagram, Service Contract Diagram, and Services Architecture Diagram. Each of the diagrams shown in this tutorial are derived from examples shown in the (2022-2023) edition of the Service Oriented Design (SOD) course at Vrije Universiteit Amsterdam, involving a "CityCar2Go" B2B (Business to Business) Service Network and the participants and services that are involved in the network.

### The tutorials are divided into four sections:

1. How to draw a Service Interface Diagram

2. How to draw a Participant Diagram

3. How to draw a Service Contract Diagram (Video Tutorial Included for the SOD Course)

4. How to draw a Services Architecture Diagram (Video Tutorial Included for the SOD Course)

### Each section will have a similar structure providing the following information in order:

1. Information about the diagram, detailing what the diagram is used for and what it represents.

2. Table of notations involved involved in the drawing of the diagram, detailing the elements of the diagram, what each notation represents and what it defines.

3. Step-by-step guide on how to draw the diagram in diagrams.net/draw.io desktop application.

Throughout the tutorials, GIF animations will be used to provide the user with additional visual guidance on how to setup the SoaML extension and draw SoaML diagrams using the SoaML libraries.

**Note:** viewing the GIF animations in full screen by clicking will provide a better quality viewing experience.

## 1 - Drawing a Service Interface Diagram

### What is a Service Interface Diagram?

---

<img src="Images/Templates/service-interface.png" width="400"/>

**Figure 1: Service Interface Diagram for an Eco-Statistics Service**

To understand what the SoaML Service Interface Diagram is about, let us be reminded that for a service provider to provide a service to a service consumer, the service provider must implement an interface for the consumer to establish a communication channel with the service provider. For a connection to be established between a service provider and a service consumer, the service provider must define the messages (signals and operations) that it can receive from the consumer by implementing a provided interface for the consumer and define the messages that it expects to be able to send back to the consumer (callbacks in a bi-directional interface) by specifying the provided interface that the consumer is to implement (modeled as a required interface from the perspective of the service provider).

The SoaML Service Interface Diagram specifies the interface that the service provider offers to provide the service logic that it owns to the service consumer and the interface that it expects the consumer to implement to receive callbacks from the provider; this defines a service with a bi-directional protocol. However, the SoaML Service Interface Diagram also allows for modeling a uni-directional interface known as a Simple Interface. In a Simple Interface Diagram, the service provider only specifies its interface to the consumer. It does not perform any callbacks to the consumer, defining a service with a uni-directional protocol.

Additionally, the Service Interface Diagram defines the roles that each participant involved within the service takes. In a bi-directional service, one participant may take the role of a service provider, thus implementing the specified provided interface in its service port. On the other hand, one participant may take the role of a service consumer, thus implementing the specified required interface in its service port.

Overall, the Service Interface Diagram defines the interactions between all of the participants involved in the service.

### SoaML Service Interface Diagram Notations

---

| Notation                                                                                                           | Name                   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------ | :--------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <img src="Images/Notations/Interface/service-interface.png" alt="Service Interface" width="200"/>                  | Service Interface      | The Service Interface specifies the interface the service provider will implement through a realization association between itself and the **Provided Interface**. A bi-directional service will also specify the interface that the service provider expects from the service consumer by associating itself to the Required Interface with a usage association. Additionally, it defines the participants involved in the service and how they establish communication with one another.                                                  |
| <img src="Images/Notations/Interface/si-interface-cport.png" alt="Interface with Consumer Interface" width="200"/> | Required Interface     | This represents the Required Interface of the service provider, which represents the interface that the service provider expects from the service consumer to allow for the service provider to perform callbacks to the service consumer. The interface is stereotyped as "Consumer" to indicate that the service consumer will implement this interface as its **Provided Interface**. Additionally, the Required Interface defines the set of messages that the service consumer can receive back from the service provider (callbacks). |
| <img src="Images/Notations/Interface/si-interface-pport.png" alt="Provided Interface" width="200"/>                | **Provided Interface** | This represents the **Provided Interface** of the service provider, the interface is stereotyped as "Provider" which indicates that the service provider will implement this interface to provide the service that it owns to the service consumer. The service consumer will use this interface as its Required Interface. Additionally, the **Provided Interface** defines the set of messages that the service provider can receive from the service consumer when the service consumer uses the service owned by the service provider.  |
| <img src="Images/Notations/Interface/si-participant-cinterface.png" alt="Consumer Role" width="200"/>              | Consumer Role          | This represents the role of a service consumer participant within a service. The service consumer's role is typed by the Required Interface.                                                                                                                                                                                                                                                                                                                                                                                                |
| <img src="Images/Notations/Interface/si-participant-pinterface.png" alt="Provider Role " width="200"/>             | Provider Role          | This represents the role of a service provider participant within a service. The service provider's role is typed by the specified Provided Interface.                                                                                                                                                                                                                                                                                                                                                                                      |
| <img src="Images/Notations/Interface/si-participant-nointerface.png" alt="Participant Role" width="200"/>          | Participant Role       | This represents the service consumer participant's role in a uni-directional Simple Interface Diagram where only one of the participants will implement a Provided Interface since message exchanges are asynchronous, allowing only a single direction from the service consumer to the service provider.                                                                                                                                                                                                                                  |
| <img src="Images/Notations/Interface/connector.png" alt="Connector" width="200"/>                                  | Connector              | This is an association used to connect the Required Interface to the Provided Interface                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| <img src="Images/Notations/Interface/realization.png" alt="Realization" width="200"/>                              | Realization            | This is the association between the Service Interface and the Provided Interface to indicate that the Service Interface implements the interface.                                                                                                                                                                                                                                                                                                                                                                                           |
| <img src="Images/Notations/Interface/usage.png" alt="Usage" width="200"/>                                          | Usage                  | This is the association between the Service Interface and the Required Interface to indicate that the Service Interface uses the interface as a Required Interface.                                                                                                                                                                                                                                                                                                                                                                         |
| <img src="Images/Notations/Interface/si-signal.png" alt="Signal" width="200"/>                                     | Signal                 | This is a message that can be added to the set of defined messages that the service provider will receive or send in the specified interfaces.                                                                                                                                                                                                                                                                                                                                                                                              |

### How to draw a Service Interface Diagram in diagrams.net

---

1. Create a new diagram in diagrams.net and give it the name of the Service that you are modeling (e.g. Eco-Statistics Service).

2. Rename the page to any name you want (i.e. Service Interface Diagram).<br><br>
   <img src="Images/Tutorial Images/Service Interface/1.gif"><br><br>

3. We will be drawing the Service Interface Diagram for a bi-directional **"Eco-Statistics Service"**, a service within the "CityCar2Go" service network. Start by navigating to the **SoaML-Interface** Library an selecting the **"Service Interface"** element. Drag and drop the element onto the canvas.<br><br>
   <img src="Images/Tutorial Images/Service Interface/2.gif"><br><br>

4. Rename the **Service Interface** element to "Eco-Statistics Service".<br><br>
   <img src="Images/Tutorial Images/Service Interface/3.gif"><br><br>

5. Next, we want to specify the **Provided Interface** that the service provider implements. To do this, navigate to the **SoaML-Interface** Library and select the **"Provided Interface"** element. Drag and drop the element onto the canvas, above the **Service Interface** Element. Give the **Provided Interface** the name "StatCenter", this will be the type of the Service Provider's role.<br><br>
   <img src="Images/Tutorial Images/Service Interface/4.gif"><br><br>

6. The **Provided Interface** should specify the set of messages that the service provider can receive from the service consumer when the consumer is using the specified service. Our **Provided Interface** for the "Eco-Statistics" Service must specify the public operations "requestStat()" to represent an optional interaction by the consumer, requesting for a specific Eco-Statistic (i.e. Carbon Emissions, Gas Usage, Nitrogen Emission etc.) and "requestFullReport()" to represent the required interaction by the consumer, requesting for a full report of the Eco-Statistics. To specify the first operation, simply rename the Signal element inside the **Provided Interface** to "+requestStat()".<br><br>
   <img src="Images/Tutorial Images/Service Interface/5.gif"><br><br>

7. Then, we need to add another operation to the **Provided Interface** for the "requestFullReport()" operation. To do this, navigate to the **SoaML-Interface** Library and select the "Signal" element. Drag and drop the element onto the **Provided Interface** element, below the "requestStat()" operation. Give the operation the name "+requestFullReport()".<br><br>
   <img src="Images/Tutorial Images/Service Interface/6.gif"><br><br>

8. Finally, we'll have to give the **Service Interface** a Realization Association with the **Provided Interface** since the service provider will implement the **Provided Interface**. To do this, navigate to the **SoaML-Interface** Library and select the "Realization" element. Link the head of the arrow to the **Provided Interface** and the arrow's tail to the Service Interface. We may remove the association's label by clicking on the label and pressing the delete key to prevent the diagram from cluttering.<br><br>
   <img src="Images/Tutorial Images/Service Interface/7.gif"><br><br>

9. Next, we want to specify the Required Interface that the service provider uses. To do this, navigate to the **SoaML-Interface** Library and select the "Required Interface" element. Drag and drop the element onto the canvas, next to the **Provided Interface** element. Give the Required Interface the name "StatConsumer"; this will be the Service Consumer's Role type.<br><br>
   <img src="Images/Tutorial Images/Service Interface/8.gif"><br><br>

10. The Required Interface should specify the set of messages that the service provider can send back to the consumer. Our Required Interface for the "Eco-Statistics" Service must specify the public operations "stat()" and "fullReport()" to denote the service provider returning of the requested data to the service consumer. To specify the first operation, rename the Signal element inside the Required Interface to "stat()".<br><br>
    <img src="Images/Tutorial Images/Service Interface/9.gif"><br><br>

11. Then, we need to add another operation to the required interface for the "fullReport()" operation. To do this, navigate to the **SoaML-Interface** Library and select the "Signal" element. Drag and drop the element onto the Required Interface, below the "+stat()" operation. Rename the Signal element to "+fullReport()".<br><br>
    <img src="Images/Tutorial Images/Service Interface/10.gif"><br><br>

12. Finally, we'll have to give the **Service Interface** a Usage Association with the Required Interface since the service provider will use the Required Interface. To do this, navigate to the **SoaML-Interface** Library and select the "Usage" element. Link the association the same way as it was done for step 8.<br><br>
    <img src="Images/Tutorial Images/Service Interface/11.gif"><br><br>

13. We'll have to specify the Service Provider's Role within the service. To do this, navigate to the **SoaML-Interface** Library and select the "Provider Role" element. Drag and drop the element into the **Service Interface** element, preferably on the same side as the **Provided Interface** element. Give the Provider Role a type of "StatCenter" to indicate that the Service Provider's role is typed by the **Provided Interface**.<br><br>
    <img src="Images/Tutorial Images/Service Interface/12.gif"><br><br>

14. Next, we'll have to specify the Service Consumer's Role within the service. To do this, navigate to the **SoaML-Interface** Library and select the "Consumer Role" element. Drag and drop the element into the **Service Interface** element, preferably on the same side as the Required Interface element. Give the Consumer Role a type of "StatConsumer" to indicate that the Service Consumer's role is typed by the Required Interface.<br><br>
    <img src="Images/Tutorial Images/Service Interface/13.gif"><br><br>

15. Connect the participant roles by navigating to the **SoaML-Interface** Library and selecting the "Connector" element, then linking the 2 roles to each other. We may remove the association's label by clicking on the label and pressing the delete key to prevent the diagram from cluttering.<br><br>
    <img src="Images/Tutorial Images/Service Interface/14.gif"><br><br>

16. We have now completed the **Service Interface** Diagram for the "Eco-Statistics" Service. Save the diagram by going to File > Save As... then selecting the location you want to save the diagram and the format that you want to save the diagram as.<br><br>
    <img src="Images/Tutorial Images/Service Interface/15.png" width="400px"><br><br>

## 2 - Drawing a Particpant Diagram

### What is a Participant Diagram?

---

<img src="Images/Tutorial Images/Service Participant/template-participant.png" width="500" height="200">

**Figure 2: Participant Diagrams for a Service Provider named "Environmental Agency" and a Service Consumer named "Municipality"**

Service Participant Diagrams model the Participants that are defined by a Service Interface Diagram or a Simple Interface Diagram. Each participant represents software components, organizations, systems, or individuals that provide and use services. The ports of each Participant and their interfaces represent a service that is being offered or requested.

This diagram acts as an extension to the Service Interface Diagram, representing the roles that are defined as Participants represented by a UML Interface diagram stereotyped by "\<\<Participant\>\>". While the Service Interface Diagram is modeled from the perspective of the service provider, the Participant Diagram is drawn from perspectives of each participants, where the Participant providing a service implements the **Service Interface** as its Service Port, and the specified Required Interface and **Provided Interface** from the Service Interface Diagram as the Required Interface and **Provided Interface** of its service port respectively. On the other hand, the Participant using the service will conjugate the modeled Service Interface Diagram, using the **Service Interface** as a Request Port, and implementing the Required Interface as the **Provided Interface** of its Request Port.

The **SoaML-Participant** library enables us to model a Participant as a UML interface, indicating that it is a Participant within a bi-directional service, and model a Participant as a UML class, indicating that it is a Participant within a uni-directional service. Additionally, the library allows us to model the architecture of a Participant to specify the internal components that are involved in providing the Participant with a capability to offer or use a service.

### SoaML Participant Diagram Notations

---

| Notation                                                                                                | Name                              | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="Images/Notations/Participant/participant.png" alt="participant" width="200"/>                 | Participant                       | The Participant notation is a UML Interface that defines a Participant within a service. This participant may implement a Service Port to provide a service, or implement a Request Port to request and use a service. Participants can be involved in multiple services and may implement multiple Service Ports and Request Ports, assuming the role of a service provider or service consumer in each service.                                                                                                                                                                    |
| <img src="Images/Notations/Participant/p-architecture.png" alt="participant architecture" width="200"/> | Participant Services Architecture | This represents the Participant as a UML Composite structure to model how a Participant fullfill their roles in one or multiple Service Contracts in order order to offfer a defined Service, or how the Participant may delegate the the fulfillment of its roles within service contracts to one or multiple other participants. The Participant Services Architecture will then offer the service through a Service Port. The Participant Services Architecture must be combined with tools within the \*\*SoaML-ServicesArchitecture library.                                    |
| <img src="Images/Notations/Participant/p-class.png" alt="participant class" width="200"/>               | Participant Class                 | Participants are modeled as UML classes when they are involved in uni-directional services modeled as a Simple Interface Diagram.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| <img src="Images/Notations/Participant/bi-port.png" alt="bi-directional port" width="200"/>             | Bi-directional Port               | This representation of a Service Interface and its Required and **Provided Interface** in a Participant Diagram. The UML Port notation denotes the **Service Interface** part of a **Service Interface** while the 2 attached interfaces denotes the specified required and provided interface form the **Service Interface** Diagram. The "\<\<Stereotype\>\>" label denotes that the Bi-directional Port can be stereotyped as a Service Port representing a **Service Interface**, or a Request Port representing a conjugated **Service Interface** being used by a participant. |
| <img src="Images/Notations/Participant/r-port.png" alt="request port" width="200"/>                     | Request Port                      | This represents a conjugated **Service Interface** with, the Required Interface of the Request Port is typed by the **Provided Interface** that a **Service Interface** Implements.                                                                                                                                                                                                                                                                                                                                                                                                  |
| <img src="Images/Notations/Participant/s-port.png" alt="service port" width="200"/>                     | Service Port                      | This Represents a **Service Interface** that is being used by a Participant to offer a service to others, the **Provided Interface** on the Port is typed by the **Provided Interface** that is implemented by a **Service Interface**.                                                                                                                                                                                                                                                                                                                                              |
| <img src="Images/Notations/Participant/r-interface.png" alt="required interface" width="200"/>          | Required Interface                | Represents a point of interaction for another participant that provides the type of the service requested.                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| <img src="Images/Notations/Participant/s-interface.png" alt="provided interface" width="200"/>          | **Provided Interface**            | Represents a point of interaction for another participant that requests for the type of service provided.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

### How to draw a Participant Diagram in diagrams.net

---

1. Continuing from our modeling of the Service Interface Diagram, create a new page for the Participant Diagrams. Name this page after the diagram you are trying to model (i.e., "Participant Diagram").<br><br>
   <img src="Images/Tutorial Images/Service Participant/1.gif"><br><br>

2. Our first step to drawing the diagram is to add a Participant, navigate to the **SoaML-Participant** library, select **"Participant"**, and drag it onto the canvas.<br><br>
   <img src="Images/Tutorial Images/Service Participant/2.gif"><br><br>

3. We will be modeling the Service Consuming Participant. Name This Participant "Municipality." This Participant will consume the "Eco-Statistics" Service provided by the Service Provider.<br><br>
   <img src="Images/Tutorial Images/Service Participant/3.gif"><br><br>

4. In the Service Interface Diagram, we have defined the "Eco-Statistics" Service as a **Service Interface** that is to be implemented by a Service Provider / Used by a Service Consumer to request the service. We have also specified that the Service Provider will implement the Required Interface that was specified in the Service Interface Diagram as their **Provided Interface**.<br><br>
   To model the **Service Interface** that the Consumer will use, we must navigate to the **SoaML-Participant** library and select the **"Bi-directional Port"** element. Drag the element onto any outer edge of the Participant.<br><br>
   <img src="Images/Tutorial Images/Service Participant/4.gif"><br><br>

5. To make it easier to interact with the different parts of the Port, ungroup the Port by right-clicking on the Port and selecting "Ungroup".
   <br><br>
   <img src="Images/Tutorial Images/Service Participant/5.gif"><br><br>

6. Since The Participant "Municipality" is a Service Consumer, it will implement the Port as a **Request Port**, give the Port a stereotype "\<\<Request\>\>" to denote that it is a **Request Port**.<br><br>
   <img src="Images/Tutorial Images/Service Participant/6.gif"><br><br>

7. The Request Port represents a **Service Interface** in a SoaML Participant Diagram. We'll have to name it after the **Service Interface** we've modeled previously in Part 1 of the tutorial. Name the Request Port "Eco-Statistics Service".<br>  
   <img src="Images/Tutorial Images/Service Participant/7.gif"><br><br>

8. The Service Consumer implements the **Provided Interface** of the **Service Interface** as the **Required Interface** of its **Request Port** since it conjugates the Service Port, name the **Provided Interface** "StatCenter".<br><br>
   <img src="Images/Tutorial Images/Service Participant/8.gif"><br><br>

9. The Service Consumer implements the **Required Interface** of the **Service Interface** as the **Provided Interface** of its **Request Port**, name the **Provided Interface** "StatConsumer".<br><br>
   <img src="Images/Tutorial Images/Service Participant/9.gif"><br><br>

10. Suppose that the Participant named "Municipality" consumes another service that provides "Location Awareness Service" capabilities. The Service Provider of the "Location Awareness Service" will offer the service through a **Provided Interface** called "LocationProvider" and will expect the Consumer to implement a "LocationRequestor" interface to interact with the Provider.
    <br><br>We'll have to model this service as a **Request Port** by following the same rules stated in steps 4-9. You may have to adjust the diagram to make it look more presentable.<br><br>
    <img src="Images/Tutorial Images/Service Participant/10.gif"><br><br>

11. Additionally, we have to model the Service Providing Participant (Service Provider) to show how the interfaces between 2 Participants can be connected if they are compatible. Since the Municipality conjugates the Service Interface, we must reverse the conjugation for the Service Provider Participant. <br><br>Create a **Participant** named "Environmental Agency" and give it a **Service Port** with the same name as the **Service Interface** from Part 1, with a **Required Interface** named "StatConsumer" and a **Provided Interface** named "StatCenter". You may have to make some adjustments to make the model more readable.<br><br>
    <img src="Images/Tutorial Images/Service Participant/11.gif"><br><br>

12. We can now connect the compatible interfaces of the 2 Participants to represent an interacting pair of Participants within the "Eco-Statistics" Service. These Participants will interact by using or providing capabilities to each other, which will then progress to fulfilling a service, which can be a goal tied to a business. <br><br>
    <img src="Images/Tutorial Images/Service Participant/12.gif"><br><br>

## 3 - Drawing a Service Contract Diagram

### What is a Service Contract Diagram?

---

<img src="Images/Tutorial Images/Service Contract/template-contract.png" width="400">

**Figure 3: Service Contract Diagram for the "Eco-Statistics" Service**

To understand what a Service Contract Diagram is, we need to understand the definition of a Service contract within SOA Systems. The Service Contract defines the terms, conditions, and interfaces of participants involved in enacting the service. Additionally, a Service Contract will define the order of participant interactions. The interactions of participants depend on their roles within a service. Each Participant is obliged to participate in enacting a service if they play a role specified by the Service Contract. The service is enacted when all participants have fulfilled their roles within the service by providing or using the signals and operations specified in their interfaces.

Previously, we have learned how to model 2 out of the 3 ways to specify a service (Simple Interface and Service Interface), now we move on to modeling the Service Contract approach for services. The SoaML Service Contract Diagram models each Participant's roles within the service specified by the UML collaboration. Additionally, SoaML Service Contract Diagrams may be accompanied by the participants that are bound within the Service Contract, which are modeled as interfaces stereotyped by "\<\<Provider\>\>" or "\<\<Consumer\>\>". The accompanying interfaces specify the messages that are exchanged between the participants that are involved in the enactment of the service; the order of the messages exchanged is defined by a UML Sequence Diagram, which usually accompanies a Service Contract Diagram to show the order of interactions between participants in the enactment of a service.

Our SoaML-ServiceContract library provides us with the tools to model a Service as a Service Contract Diagram, specifying the participants involved \(shown inside the Service Contract)\ and their roles. The library also provides us with additional notations that extend the capabilities of a UML Sequence Diagram to model the choreography of the service. Furthermore, other libraries, such as the SoaML-Participant library and SoaML-Interface library, can be utilized to extend the details of the service model by a Service Contract Diagram.

### SoaML Service Contract Diagram Notations

---

| Notation                                                                                               | Name                    | Description                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------ | :---------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="Images/Notations/Contract/s-contract.png" alt="service contract" width="200"/>               | Service Contract        | Represents the Service Contract, defining the roles that participants play within the enactment of a service. The roles of each participant will be contained within this diagram.                                                                                                                                                                                                                                                                       |
| <img src="Images/Notations/Contract/consumer.png" alt="consumer" width="200"/>                         | Consumer Role           | Represents a Participant Playing the role of the service consumer within the enactment of the service. The semi-circle on the top right denotes that the participant implements the required interface from the perspective of the service provider.                                                                                                                                                                                                     |
| <img src="Images/Notations/Contract/provider.png" alt="provider" width="200"/>                         | Provider Role           | Represents a Participant Playing the role of the service provider within the enactment of the service. The circle on the top right denotes that the participant implements the provided interface.                                                                                                                                                                                                                                                       |
| <img src="Images/Notations/Contract/i-contract.png" alt="nested service contract" width="200"/>        | Nested Service Contract | Represents a Service Contract that needs to be fulfilled to fulfill the roles that each Participant in the service play.                                                                                                                                                                                                                                                                                                                                 |
| <img src="Images/Notations/Contract/s-channel.png" alt="service channel" width="200"/>                 | Service Channel         | This represents a communication channel between the 2 participants. When it connects 2 participants, it denotes that the participants with a service channel between them can exchange messages (signals or operations). The exchange of messages can be further specified in UML behavior diagrams.                                                                                                                                                     |
| <img src="Images/Notations/Contract/c-lifeline.png" alt="consumer lifeline" width="100" height="200"/> | Consumer Lifeline       | This represents the lifeline of the Consumer participant. We can then model the messages sent by the participant as a solid line with a filled arrow labeled by the operation and pointing away from the participant and toward another participant or itself. The circle on the right is added as an extension to the UML profile. This circle denotes that the participant implements an interface to send the message (operation call) to a provider. |
| <img src="Images/Notations/Contract/p-lifeline.png" alt="provider lifeline" width="100" height="200"/> | Provider Lifeline       | Represents the lifeline of a Provider participant. Since a provider can make a callback (return message in response to an operation call) to a consumer, this callback message is denoted as a dashed line with an unfilled arrow, labeled by the return message, pointing back towards the caller (consumer). Additionally, a provider can also make a call to another provider; for instance, in a multi-party service.                                |

### How to draw a Service Contract Diagram in diagrams.net

---

1. Start by creating a new page or new diagram and name it "Service Contract Diagram".<br><br>

2. In this tutorial, we will define the "Eco-Statistics" service through the third approach to defining services in SOA known as the "Contract Based Approach". To start off, lets add the Service Contract UML collaboration to the canvas.<br><br>Navigate to the **"SoaML-ServiceContract"** library and drag the **"Service Contract"** element onto the canvas and name the **Service Contract** "Eco-Statistics".<br><br>
   <img src="Images/Tutorial Images/Service Contract/2.gif"/>

3. As previously specified by the **Service Interface** approach to defining the "Eco-Statistics" service, there were 2 **Participant Roles** in the service. We will have to specify this also for the **Service Contract** Approach.<br><br>Specify the Consumer Participant's role in the Service by navigating to the **"SoaML-ServiceContract"** library and dragging the **"Consumer Role"** element into the left side of the **Service Contract**.<br><br>
   <img src="Images/Tutorial Images/Service Contract/3.gif"/>

4. Give it a role "Consumer" and type the role as "StatConsumer", this is the name of the **Required Interface** that we have specified in Part 1 of the tutorial. Recall that the role of a Participant is typed by the Interface that they implement.<br><br>
   <img src="Images/Tutorial Images/Service Contract/4.gif"/>

5. <img src="Images/Tutorial Images/Service Contract/5.gif"/>

6. <img src="Images/Tutorial Images/Service Contract/6.gif"/>

7. <img src="Images/Tutorial Images/Service Contract/7.png" width="800"/>

## 4 - Drawing a Services Architecture Diagram

### What is a Services Architecture Diagram?

### SoaML Services Arthitecture Diagram Notations

| Notation                                                                                                       | Name                      | Description                                                                                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------- | :------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <img src="Images/Notations/Services Architecture/SA.png" alt="Service Interface" width="200"/>                 | Services Architecture     | ServicesArchitecture describes how a network of participants work together by providing and consuming services to fulfill a purpose. Where each services are expressed as service contracts |
| <img src="Images/Notations/Services Architecture/SC.png" alt="Interface with Consumer Interface" width="200"/> | Internal Service Contract | Service Contract gives a description of how participants should interact in order to enact a service                                                                                        |
| <img src="Images/Notations/Services Architecture/PI.png" alt="Service Interface" width="200"/>                 | Internal Participant      | Internal role within a services architecture, where the role of a participant is typed by the interface that they implement                                                                 |
| <img src="Images/Notations/Services Architecture/PE.png" alt="Service Interface" width="200"/>                 | External Participant      | External role that is involved in the services architecture. Role of participant is typed by the interface that they implement                                                              |
| <img src="Images/Notations/Services Architecture/role-binding.PNG" alt="Service Interface" width="200"/>       | Role Binding              | A role binding attaches a participant with a compatible interface to the service contract within the architecture. Giving the participant its role within the Services Architecture         |

### How to draw a Services Architecture Diagram in diagrams.net

1.  <img src="Images/Tutorial Images/Services Architecture/1.gif"/>

2.  <img src="Images/Tutorial Images/Services Architecture/2.gif"/>

3.  <img src="Images/Tutorial Images/Services Architecture/3.gif"/>

4.  <img src="Images/Tutorial Images/Services Architecture/4.gif"/>

5.  <img src="Images/Tutorial Images/Services Architecture/5.gif"/>

6.  <img src="Images/Tutorial Images/Services Architecture/6.gif"/>

7.  <img src="Images/Tutorial Images/Services Architecture/7.gif"/>

8.  <img src="Images/Tutorial Images/Services Architecture/8.gif"/>

9.  <img src="Images/Tutorial Images/Services Architecture/9.gif"/>

10. <img src="Images/Tutorial Images/Services Architecture/10.gif"/>

11. <img src="Images/Tutorial Images/Services Architecture/11.gif"/>

12. <img src="Images/Tutorial Images/Services Architecture/12.png"/>

13. <img src="Images/Tutorial Images/Services Architecture/13.png"/>

14. <img src="Images/Tutorial Images/Services Architecture/14.png"/>

# SoaML Templates
