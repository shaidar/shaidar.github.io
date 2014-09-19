---
layout: post
title: "Application Virtualization, a Higher Education Reality"
modified:
categories: 
excerpt:
tags: [AppV, ThinApp, VMware, Citrix, Virtualization, VDI, Desktop Computing, IT Higher Education, Reality]
image:
  feature:
date: 2010-01-31T17:41:00-04:00
---
The enormous amount and diversity of applications found in Higher Education makes managing it quite a feat. Separating the application from its underlying components and viewing things from a layered perspective, there’s the application itself, user workspace, storage, operating system and hardware (Dell, HP, Thin clients like Wyse) to name most of them. Unfortunately all the hype is centered on Virtual Desktop Infrastructure (VDI) and “Green IT” that Managers seem to be convinced that virtualizing their desktop environment would also solve their application layer problems, but would it?  What are the problems affecting traditional software installations? What are the challenges of the “new” model?

#### Shortcomings of the “traditional” model

* Application incompatibilities: The more applications installed on a machine, the higher the possibility of application incompatibilities due to varying pre-requisites in some cases. An example would be two different apps requiring different versions of java or one application overwriting a Dynamic Link Library (dll) file used by a previously installed app.
* Patching or upgrading apps: Unless the infrastructure is already in place to update or patch the installed apps, reimagining the computers to apply an upgrade is the optimal way. Even with a solution that pushes out updates or patches, a tremendous amount of regression testing is needed before deploying the new image.
* Failure to run different versions of the same application: Corporate America might not view this as a major obstacle, but in Higher Education there’s a need to run multiple versions of the same application to ease the transition for users. Running multiple versions of the same application helps in training users on the new version and reaching a certain comfort level before retiring the older version. At times there’s also a need to keep an older version because some of the available textbooks still refer to it.

#### What is Application Virtualization?

The concept of virtualization can be traced back to the idea of “time sharing” coined by Christopher Strachey in the early 1960s. Strachey was referring to multi-programming where one user would be working on a program while the other would be debugging another program concurrently. Application Virtualization is the abstraction of the underlying layer, the Operating System (OS), and is accomplished by tricking the application into believing that it’s residing and interacting directly with the OS, when in fact it’s running in its own isolated virtual environment.  
Virtualized applications can run in one of two environments:
1. Clients machine thus using local resources.
2. Terminal Server (TS) where processing cycles are provided by the server and the end user establishes a remote session.

#### What can Application Virtualization do for me?
The majority of the problems discussed above regarding the application layer can be resolved through application virtualization.   
Since the virtualized apps run in their own sandboxed environment, each app “believes” that it’s running on its own in the OS thus application incompatibilities don’t arise.   
In addition because of this “bubble” environment, each application can be bundled with all its prerequisites thus allowing the end user to run multiple versions of the same software on the same machine. Some institutions used application virtualization to provide Microsoft Office 2003 and 2007 simultaneously. During the fall semester, Office 2003 was setup as the default suite while Office 2007 was available for access to anyone who’s interested. Then in the spring semester, Office 2007 became the default suite while Office 2003 remained for those who still haven’t made the transition.   
Since applications are locally installed on the computer, upgrading or patching an app becomes a matter of repackaging the app and distributing it to the clients using the means available. SPSS, a statistical application, came out with a critical patch and through application virtualization, the packaged app was upgraded and access to it was quickly provided.  
Furthermore, the modular/layered approach of decoupling the apps from the OS will allow the IT Manager the freedom of investigating solutions to better manage the other layers without the hassle of trying to find a non-existent solve all type of solution. Based on the vendor and application virtualization solution in place, some of the added benefits are the centralization of software distribution, application usage statistics, license management, and the ability to manage application access and authorization. 
Prior to application virtualization, one of the major obstacles to Server Based Computing (SBC) is offline use. The majority of the existing application virtualization solutions handle offline use by streaming and caching the application locally or by creating a complete self-encompassed package that can run with no strings attached.

#### Application Virtualization and its Challenges
Any new system has a learning curve and some shortfalls and application virtualization is no different.   

* **Virtual App, maybe not!**    
Before jumping into application virtualization the main takeaway is that no matter what vendor/solution is chosen, not all applications can be virtualized. Similar to server virtualization where its inadequate in some instances and a physical server might be required, some apps have to be installed and can’t be virtualized. Those are mainly the apps dealing with system level drivers or in some cases COM+ objects. For example, Zoomtext, an Ai Squared product used for screen magnification can’t be virtualized at this point due to its manipulation of the video drivers. Hence, the move to application virtualization will still require maintaining an existing software distribution solution to manage the apps that can’t be virtualized unless the apps can be bundled with the image.  

* **Vendors and license agreements**    
The added benefits of license management, application usage stats and the centralization of application distribution will necessitate a revision of some license agreements and possibly a reduction in the number of licenses in other cases. A good amount of the software vendors either aren’t aware of application virtualization or haven’t adjusted their licensing models to take it into consideration. So, when trying to get the optimal amount of licenses or renegotiating a license agreement, things might get tricky dealing with the vendor. Also, some vendors have different licenses thus pricing to run their software on TS. Hence, when putting a budget together for an application virtualization deployment, its vital to decide what apps will be offered how.  

* **Complexity and training**  
<br>
End Users  
If the virtual app is running locally on the end users machine, training is quite minimal or even non-existent. Whether an application is virtual or locally installed, all the average user cares about is whether the app is launched when he/she double clicks on the shortcut. Some training is needed in case a laptop is involved and offline access to an app is required. In that case, the user would need to locally cache the app before going offline.
If on the other hand the virtual app is hosted on a TS and connecting to a remote session is new to your environment, some training might be needed.  
<br>
IT Admins  
Based on the size of the institution and the number of applications being virtualized, a full time employee is needed to package the apps and keep things updated. Again based on the purchased solution, new infrastructure will be needed mainly composed of application servers, database server, and management console taking into consideration redundancy and load balancing. Other solutions allow you to create the virtual app and use an existing software distribution solution. In those cases, there’s very minimal overhead to maintain. 
Personally, the biggest challenge is finding resources and experts on the subject matter, but I have to admit that in the past two years application virtualization adoption has grown tremendously and so has the number of experts and consultants.   

* **Faculty Buy-In**  
Apart from the technical challenges, faculty buy-in is key in any successful implementation.  

* **Service Name vs. Product Name**
When marketing the project at your institution I recommend not using the product name for the provided service. Vendors get sold, products get renamed and it will create a lot of confusion when the service keeps getting a name change.  

* **Workflow and software ordering**  
Application virtualization doesn’t necessarily mean centralizing software distribution but in case that’s the chosen route, then a reevaluation of software ordering, distribution, assignment, updating, and license negotiating processes would need to be adjusted and possibly a new workflow established.

**Some Possible Solutions**  
<br>
The major players in this field in alphabetical order are:

* Citrix XenApp  
XenApp, similar to Microsoft’s App-V is an agent-based solution that offers client and server side application virtualization. In addition, with the new release of XenApp, if an app can’t be virtualized it can be installed on a Virtual Machine (VM) and access to it provided to the end user. In my opinion, that’s a sign of product maturation by accepting the fact that not all apps can be virtualized and providing a solution. Again, similar to App-V, the application is streamed and cached on the client, be it an end user machine or a server thus coping with the offline use dilemma.   
One of the major complaints Citrix Admins had, were the TS silos. The TS silos were a result of app compatibility and the need to have separate server farms housing different applications, but with the advent of application virtualization, the silo effect has been mitigated.   
XenApp also provides a SBC component by using a proprietary remote session protocol known as Independent Computing Architecture (ICA).

* Microsoft App-V  
In July 2007, Microsoft acquired Softricity, a company with a product called Softgrid thus entering the application virtualization market. The current product is known as Microsoft Application Virtualization or App-V for short and is part of Microsoft Desktop Optimization Pack (MDOP) offered through Software Assurance.   
App-V is an agent-based solution that offers client-side and server-side application virtualization. Once an application is “sequenced” (virtualized) and is assigned to a group of users (assigning an app to a group of computers would require Microsoft’s System Center Configuration Manager), the necessary files needed for the initial app launch can be streamed using the Real Time Streaming Protocol (RTSP) or RTSPS to the end user machine and cached locally.   
In case of Server Based Computing (SBC) where the App-V client is installed on a TS, the end user would use a web portal to authenticate and launch an application be establishing a remote desktop session to the server.  

* VMware ThinApp  
VMware acquired Thinstall to add application virtualization to its repertoire.
Unlike XenApp and App-V, ThinApp is an agent-less solution that has an embedded virtual OS along with the packaged app. ThinApp doesn’t have an application streaming or distribution mechanism. The packaged app is self-sufficient and can be pushed out just like any other file. As opposed to XenApp and App-V, ThinApp doesn’t need an infrastructure or an agent, but it doesn’t provide any means to distribute the virtual app. 

There are a multitude of vendors operating in the application space and have an entire suite of apps to handle the additional layers (hardware, OS, user workspace, storage) too. Citrix, to name one, has the XenDesktop product for a Virtual Desktop Infrastructure (VDI) solution or Symantec with their suite. So, before jumping on the VDI curve of “inflated expectations”, I suggest that this be treated just like any other major project by assessing the needs, test by virtualizing the main enterprise apps and look into a phased implementation.  
In conclusion, it’s not a question of virtualizing the apps or not, it’s a question of what solution works best for your environment. 
