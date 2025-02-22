# Deployment of a 3-tier application on Amazon Web Services (AWS)
When building a cloud-based application, the underlying architecture and environment are just as critical as the application itself. There are many considerations when deciding on the proper architecture of your app:

~ Scalability: How easily and/or frequently does the app need to scale up or down? How much value do you put into not having to constantly micro-manage and monitor resource usage?

~ Availability: How readily available is your app? How important is being able to go through long periods of time without failures? If failure does occur in a part of your app, how vulnerable is the rest?

~ Security: How secure is your app? How does your app handle security permissions for different parts of your app? If an attack happens in one part of your app, how vulnerable is the rest?

## Enter the AWS 3-tier architecture

<b>Why 3-tier?</b> 

This form of architecture addresses all the issues stated above. it provides increased scalability, availability, and security by spreading the application into multiple Availability Zones and separating it into three layers that serve different functions, independent of each other. If an AZ does down for some reason, the application has the ability to automatically scale resources to another AZ, without affecting the rest of the application tiers. Each tier has its own security group that only allows the inbound/outbound traffic needed to perform specific tasks.

<b>~ Web/Presentation Tier:</b> Houses the user-facing elements of the application, such as web servers and the interface/frontend. 

<b>~ Application Tier:</b> Houses the backend and application source code needed to process data and run functions. 

<b>~ Data Tier:</b> Houses and manages the application data. Often where the databases are stored. 

## System Design 

![image](https://github.com/user-attachments/assets/2795fef3-867b-4cf0-8d67-3548942e2179)

## Kindly read documentation PDF for all the steps reference of the project
