:original_name: en-us_topic_0035470099.html

.. _en-us_topic_0035470099:

Disk-intensive ECSs
===================

Overview
--------

D2 ECSs are developed based on KVM virtualization. They use local storage and provide high storage performance and intranet bandwidth for distributed Hadoop computing, large data warehouse, distributed file system, and log/data processing.

Specifications
--------------

.. table:: **Table 1** D2 ECS specifications

   +---------------+-------+--------+------------------------+----------+-----------------+----------------+-------------+-----------------------------+
   | Flavor        | vCPUs | Memory | Max./Assured Bandwidth | Max. PPS | Max. NIC Queues | Virtualization | Local Disks | Hardware                    |
   |               |       |        |                        |          |                 |                |             |                             |
   |               |       | (GiB)  | (Gbit/s)               | (10,000) |                 |                | (GiB)       |                             |
   +===============+=======+========+========================+==========+=================+================+=============+=============================+
   | d2.xlarge.8   | 4     | 32     | 4/1.4                  | 40       | 2               | KVM            | 2 x 1675    | CPU: Intel® Xeon® Gold 6151 |
   +---------------+-------+--------+------------------------+----------+-----------------+----------------+-------------+-----------------------------+
   | d2.2xlarge.8  | 8     | 64     | 6/2.8                  | 80       | 4               | KVM            | 4 x 1675    |                             |
   +---------------+-------+--------+------------------------+----------+-----------------+----------------+-------------+-----------------------------+
   | d2.4xlarge.8  | 16    | 128    | 10/5.6                 | 160      | 6               | KVM            | 8 x 1675    |                             |
   +---------------+-------+--------+------------------------+----------+-----------------+----------------+-------------+-----------------------------+
   | d2.6xlarge.8  | 24    | 192    | 15/8.5                 | 250      | 8               | KVM            | 12 x 1675   |                             |
   +---------------+-------+--------+------------------------+----------+-----------------+----------------+-------------+-----------------------------+
   | d2.8xlarge.8  | 32    | 256    | 17/11                  | 320      | 8               | KVM            | 16 x 1675   |                             |
   +---------------+-------+--------+------------------------+----------+-----------------+----------------+-------------+-----------------------------+
   | d2.15xlarge.9 | 60    | 540    | 17/17                  | 500      | 16              | KVM            | 24 x 1675   |                             |
   +---------------+-------+--------+------------------------+----------+-----------------+----------------+-------------+-----------------------------+

Scenarios
---------

-  Applications

   Disk-intensive ECSs are suitable for applications that require large volumes of data to process, high I/O performance, and rapid data switching and processing.

-  Application scenarios

   Big data computing, network file systems, data processing, MapReduce, Hadoop, and data-intensive computing

Features of D2 ECSs
-------------------

-  D2 ECSs use local disks to provide high sequential read/write performance and low latency, improving file read/write performance.
-  D2 ECSs provide powerful and stable computing capabilities, ensuring efficient data processing.
-  D2 ECSs with a vCPU/memory ratio of 1:8 process large volumes of data.
-  D2 ECSs provide high intranet performance, including high intranet bandwidth and PPS, meeting requirements for data exchange between ECSs during peak hours.
-  Each D2 ECS supports a maximum configuration of 24 local disks, 60 vCPUs, and 540 GiB memory.

.. table:: **Table 2** Specifications of a Single SAS HDD Disk Attached to a D2 ECS

   ================== ===================
   Metric             Performance
   ================== ===================
   Disk capacity      1,675 GiB
   Maximum throughput 230 MBps
   Access latency     Within milliseconds
   ================== ===================

Notes
-----

-  :ref:`Table 3 <en-us_topic_0035470099__table192771727112217>` lists the OSs supported by disk-intensive ECSs.

   .. _en-us_topic_0035470099__table192771727112217:

   .. table:: **Table 3** Supported OS versions

      +-----------------------------------+-----------------------------------------------------+
      | OS                                | Version                                             |
      +===================================+=====================================================+
      | Alma                              | Alma 8 64bit                                        |
      +-----------------------------------+-----------------------------------------------------+
      | CentOS                            | -  CentOS Stream 8.6 64bit                          |
      |                                   | -  CentOS 7.9 64bit                                 |
      |                                   | -  CentOS 7.7 64bit                                 |
      +-----------------------------------+-----------------------------------------------------+
      | Debian                            | -  Debian GNU/Linux 11 64bit                        |
      |                                   | -  Debian GNU/Linux 10 64bit                        |
      +-----------------------------------+-----------------------------------------------------+
      | EulerOS                           | EulerOS 2.5 64bit                                   |
      +-----------------------------------+-----------------------------------------------------+
      | Fedora                            | -  Fedora 35 64bit                                  |
      |                                   | -  Fedora 34 64bit                                  |
      |                                   | -  Fedora 33 64bit                                  |
      +-----------------------------------+-----------------------------------------------------+
      | OpenSUSE                          | OpenSUSE 15.3 64bit                                 |
      +-----------------------------------+-----------------------------------------------------+
      | Oracle Linux                      | -  Oracle Linux Server release 8.4 64bit            |
      |                                   | -  Oracle Linux Server release 7.6 64bit            |
      +-----------------------------------+-----------------------------------------------------+
      | Red Hat                           | -  Red Hat Enterprise Linux 7.9 64bit               |
      |                                   | -  Red Hat Enterprise Linux 6.10 64bit              |
      +-----------------------------------+-----------------------------------------------------+
      | Rocky                             | Rocky 8 64bit                                       |
      +-----------------------------------+-----------------------------------------------------+
      | SUSE                              | -  Novell SUSE Linux Enterprise Server 15 SP3 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 15 SP2 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 15 SP1 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 15 64bit     |
      |                                   | -  Novell SUSE Linux Enterprise Server 12 SP5 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 12 SP4 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 12 SP3 64bit |
      +-----------------------------------+-----------------------------------------------------+
      | SUSE-SAP                          | -  Novell SUSE Linux Enterprise Server 15 SP3 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 15 SP2 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 15 SP1 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 15 64bit     |
      |                                   | -  Novell SUSE Linux Enterprise Server 12 SP5 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 12 SP4 64bit |
      |                                   | -  Novell SUSE Linux Enterprise Server 12 SP3 64bit |
      +-----------------------------------+-----------------------------------------------------+
      | Ubuntu                            | -  Ubuntu 20.04 server 64bit                        |
      |                                   | -  Ubuntu 18.04 server 64bit                        |
      +-----------------------------------+-----------------------------------------------------+
      | Windows                           | -  Windows Server 2019 Standard 64bit               |
      |                                   | -  Windows Server 2016 Standard 64bit               |
      |                                   | -  Windows Server 2012 R2 Standard 64bit            |
      +-----------------------------------+-----------------------------------------------------+
      | openEuler                         | openEuler 20.03 64bit                               |
      +-----------------------------------+-----------------------------------------------------+

-  When the physical host where a D2 ECS is deployed becomes faulty, the ECS cannot be migrated.

-  To improve network performance, you can set the NIC MTU of a D2 ECS to **8888**.

-  D2 ECSs do not support modifying specifications.

-  D2 ECSs do not support local disk snapshots or backups.

-  D2 ECSs do not support OS reinstallation or change.

-  D2 ECSs can use both local disks and EVS disks to store data. In addition, they can have EVS disks attached to provide a larger storage size. Use restrictions on the two types of storage media are as follows:

   -  Only an EVS disk, not a local disk, can be used as the system disk of a D2 ECS.

   -  Both EVS disks and local disks can be used as data disks of a D2 ECS.

   -  A maximum of 60 disks (including VBD, SCSI, and local disks) can be attached to a D2 ECS. Among the 60 disks, the maximum number of SCSI disks is 30, and the VBD disks (including the system disk) is 24. For details, see :ref:`Can I Attach Multiple Disks to an ECS? <en-us_topic_0018073215>`

      .. note::

         The maximum number of disks attached to an existing D2 ECS remains unchanged. To attach 60 disks, enable advanced disk. For details, see :ref:`Enabling Advanced Disk <en-us_topic_0122307169>`.

   -  You are advised to use World Wide Names (WWNs), but not drive letters, in applications to perform operations on local disks to prevent drive letter drift (low probability) on Linux. Take local disk attachment as an example:

      If the local disk WWN is wwn-0x50014ee2b14249f6, run the **mount /dev/disk/by-id/wwn-0x50014ee2b14249f6** command.

      .. note::

         How can I view the local disk WWN?

         #. Log in to the ECS.

         #. Run the following command:

            **ll /dev/disk/by-id**

-  The local disk data of a D2 ECS may be lost due to some reasons, such as physical server breakdown or local disk damage. If the data reliability of your application cannot be ensured, you are strongly advised to use EVS disks to build your ECS.

-  When a D2 ECS is deleted, its local disk data is automatically deleted. Back up the data before deleting such an ECS. Deleting local disk data is time-consuming. Therefore, a D2 ECS requires a longer period of time than other ECSs for releasing resources.

-  Do not store long-term service data in local disks. Instead, back up data in a timely manner and use a high availability data architecture. Store long-term service data in EVS disks.

-  You are not allowed to buy additional local disks. The quantity and capacity of your local disks are determined according to your ECS flavor. For D2 ECSs, if additional local disks are required, buy them when creating the ECSs.
