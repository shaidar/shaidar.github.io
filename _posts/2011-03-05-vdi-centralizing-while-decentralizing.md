---
layout: post
title: "VDI, Centralizing While Decentralizing"
modified:
categories: 
excerpt:
tags: []
image:
  feature:
date: 2011-03-05T14:14:00-04:00
---
VDI abstracts the hardware, virtualizes the OS and apps, and redirects the data. So, VDI centralizes the desktop while decentralizing the individual desktop layers within the datacenter.  
<br>
That's a mouthful and it sure sounds complicated but in reality it's not. Let me pull the divide and conquer technique to make sense of things. Some people believe that VDI is no more than moving the desktop to to the data center. I previously wrote about [VDI and the new Virtual Order](/from-desks-to-data-centers) challenging that notion. I'm here again to provide yet another perspective on why VDI is more than simply moving your desktop to the data center. VDI takes a layered approach to the desktop and divides it into four major layers: 

1. Hardware
2. OS
3. Apps/Software
4. Data - User & Application  

Given that layered approach, let's tackle the opening statement:
<br> 
**VDI abstracts the hardware** by moving the desktop into the data center and granting the user the ability to access it from anywhere and from practically any device (vendor/protocol related).  
<br>
**Virtualizes the OS and apps** by mainly running the OS (Windows, Linux ... ) as a Virtual Machine on servers housed in the data center. In addition, in most instances (not all apps can be virtualized at this point), it keeps the OS layer separate from the apps layer through application virtualization.  
<br>
**Redirects Data** by means of folder redirection in its simplest implementation and there are lots of rumblings now about User Virtualization. User and Application Data are stored on file servers within the data center.  
<br>
Through the layered approach, VDI has centralized the desktop by abstracting the first layer (hardware), virtualizing layer two and three (OS and Apps) and redirecting the data, layer four (data).  
<br>
VDI centralizes the desktop while decentralizing the individual desktop layers within the datacenter.  
<br>
Through VDI, the desktop exists centrally in the data center, but due to the layered approach discussed above, the layers themselves exist in different areas of the data center. In that sense one can view VDI as virtual assembly of Desktops on login since all the different layers come together as soon as the end user logs in. 
