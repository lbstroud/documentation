.. include:: ../GLOBAL.rst

.. _deprecation:

Hosted Scalr End Support of Features Notice (**18-Mar-2019**)
=============================================================

Over the next few months, Scalr intends to cease support and deprecate from the Scalr product certain legacy functionality, as specified below. The purpose of this communication is to outline what product components are impacted, the timing and roll-out of this plan, and what you may need to do to mitigate any impact to your current operations as a result.

While we understand that the removal of these features may impact some of our customer’s current use of the product, usage of these features is minimal, and we believe this is the best decision for our product and for our customers going forward.  Over the last several major releases, Scalr has added significant strategic functionality in areas such as service catalog, orchestration/automation, policy/governance, containers, and much more. We are working on some really exciting new DevOps tools and integrations that we will be rolling out in the near future and our renewing our investment in a Hosted/SaaS Scalr offering.

Features impacted:
------------------

.. |AUTO1| image:: images/auto1.png

.. |AUTO2| image:: images/auto2.png


* **Built-in Automation - Database:** pre-built automation for common administrative and operational tasks, including MySQL, Percona, PostgreSQL and Redis built-in automation.
* **Built-in Automation - Other:** pre-built automation for common administrative and operational tasks, including Apache, Tomcat, HA Proxy, Nginx, Memcached, RabbitMQ automation.

|AUTO1| |AUTO2|

* **Scalr Role Builder:** wizard based workflow for creating Roles
* **DNS Management - Scalr Static Zones:** \*.scalr-dns.net zones that are used as static endpoints to built-in automation role.
* **DNS Management - Custom Zones:** use of Scalr to manage custom DNS zones
* **Software RAID:** Scalr functionality to create and manage software RAID storage on AWS EBS.
* **Script Parameter Interpolation:** legacy feature to declare parameters within Scalr scripts like %param%.
* **Custom Server Snapshot for Linux on AWS:** Scalr functionality to do custom snapshotting of running servers (instead of AWS CreateImage API)

Deprecation Schedule:
---------------------

+---------------------+-------------+-------------------------------------------------+----------------------------------------------+
| Feature             | Date        | Change                                          | Migration Plan                               |
+=====================+=============+=================================================+==============================================+
| Built-in Automation |  1-Apr-2019 | Users will not be permitted to create or launch | Use of Scalr orchestration and automation,   |
|                     |             | new Roles with Scalr Built-in Automation        | and product (e.g. MySQL) functionality.      |
|                     +-------------+-------------------------------------------------+                                              +
|                     |  1-May-2019 | All Built-in Automation Roles will be converted |                                              |
|                     |             | to Base Roles.                                  |                                              |
+---------------------+-------------+-------------------------------------------------+----------------------------------------------+
| Scalr Role Builder  |  1-May-2019 | Role Builder will be removed.                   | Standard processes for building Scalr Roles. |
+---------------------+-------------+-------------------------------------------------+----------------------------------------------+
| DNS Management -    | 15-Apr-2019 | Scalr will disable and remove all               | Migration to any popular DNS service such as |
| Scalr Zones         |             | \*.scalr-dns.net zones from it’s management.    | Route 53.                                    |
|                     |             | Starting from specified date these zones won’t  |                                              |
|                     |             | resolve in any IP.                              |                                              |
+---------------------+-------------+-------------------------------------------------+----------------------------------------------+
| DNS Management -    | 31-Mar-2019 | Users will not be able to add new DNS zones.    | Migration to any popular DNS service such as |
| Custom Zones        |             | Existing zones still can be managed and will    | Route 53.                                    |
|                     |             | resolve with correct IPs.                       |                                              |
+                     +-------------+-------------------------------------------------+                                              +
|                     |  1-May-2019 | Functionality will be removed completely. DNS   |                                              |
|                     |             | servers will be shut off and zones resolution   |                                              |
|                     |             | won’t work anymore.                             |                                              |
+---------------------+-------------+-------------------------------------------------+----------------------------------------------+
| Scalr RAID          |  1-May-2019 | Functionality will be removed.                  | Migrate to standard EBS volumes, or other    |
|                     |             |                                                 | storage options.                             |
+---------------------+-------------+-------------------------------------------------+----------------------------------------------+
| Scalr Script        |  1-May-2019 | Functionality will be removed.                  | Use of Scalr Global Variables                |
| Parameters          |             |                                                 |                                              |
+---------------------+-------------+-------------------------------------------------+----------------------------------------------+

Thank you for your attention to this. If you do have questions on the proposed change, please open a support ticket from the support tab in the Scalr interface.  We will send subsequent reminders on this over the next several weeks.

Regards,

Michael Lochead |BR|
VP Customer Success |BR|
Scalr
