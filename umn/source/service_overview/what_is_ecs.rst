:original_name: en-us_topic_0013771112.html

.. _en-us_topic_0013771112:

What Is ECS?
============

An Elastic Cloud Server (ECS) is a basic computing unit that consists of vCPUs, memory, OS, and Elastic Volume Service (EVS) disks. After an ECS is created, you can use it on the cloud similarly to how you would use your local PC or physical server.

ECSs support self-service creation, modification, and operation. You can create an ECS by specifying its vCPUs, memory, OS, and login mode. After an ECS is created, you can modify its specifications if necessary. ECS works with other services to provide a reliable, secure, efficient computing environment.

-  For details about the operating systems supported by ECS, see :ref:`Image Types <en-us_topic_0030828254>`.
-  For details about the login authentication mode, see :ref:`Logging In to an ECS <en-us_topic_0092494193>`.

System Architecture
-------------------

ECS works with other products and services to provide computing, storage, and network resources. You can quickly migrate and replicate existing ECSs using images.

-  ECSs can be deployed in multiple availability zones (AZs) connected with each other through an internal network. If one AZ becomes faulty, other AZs in the same region will not be affected.
-  With the Virtual Private Cloud (VPC) service, you can build your own dedicated network on the cloud. You can also set subnets and security groups within your VPC for further isolation. You can allow your VPC to communicate with the external network through an EIP (bandwidth support required).
-  With the Image Management Service (IMS), you can use an image to create ECSs. Alternatively, you can use an existing ECS to create a private image and use the private image to create the same ECSs for rapid service deployment.
-  Elastic Volume Service (EVS) provides storage space and Volume Backup Service (VBS) provides data backup and restoration functions.
-  Cloud Eye lets you keep a close eye on the performance and resource utilization of ECSs, ensuring ECS reliability and availability.
-  Volume Backup Service (VBS) allows you to create data backups for EVS disks and use the backups to restore the EVS disks. This maximizes user data correctness and security.
-  Cloud Server Backup Service (CSBS) backs up all EVS disks of an ECS, including the system disk and data disks, and uses the backup to restore the ECS.


.. figure:: /_static/images/en-us_image_0071898891.png
   :alt: **Figure 1** System architecture

   **Figure 1** System architecture

Access Methods
--------------

You can access ECS through the web-based management console or HTTPS-based application programming interfaces (APIs).

-  Accessing ECSs through APIs

   Use this method if you intend to integrate the ECSs on the cloud platform into a third-party system for secondary development. For details, see *Elastic Cloud Server API Reference*.

-  Accessing ECSs through the management console

   Use this method if you are not required to integrate ECSs with a third-party system.

   Log in to the management console with your account and choose **Elastic Cloud Server** on the homepage.
