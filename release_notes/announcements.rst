.. include:: ../GLOBAL.rst

.. _scalr_announcements:

Announcements
==============

Built-In Automation Deprecation
-------------------------------

The following features will no longer be available as of Scalr 7.15.0:

* Role Builder
* Built-In Automation Roles - This will only impact NEW Farm Roles, existing Farm Roles will continue to work.
* Script Parameters - Global Variables in scripts has replaced this functionality. 

Hosted Scalr End Support of Features Notice (**18-Mar-2019**)
-------------------------------------------------------------

Over the next few months, Scalr intends to cease support and deprecate from the Scalr product certain legacy functionality, as specified below. The purpose of this communication is to outline what product components are impacted, the timing and roll-out of this plan, and what you may need to do to mitigate any impact to your current operations as a result.

Please review this :ref:`Deprecation Notice <deprecation>` for full details of the features that are being removed and migration plan for each one.

Suse Support
-------------

Suse 11.3, 11.4, and 12.x are now officially supported by Scalarizr. The following software automation tools will be supported:

* Chef
* Ansible

Ubuntu 18.04 Support
--------------------

Ubuntu 18.0.4 is now officially supported by Scalarizr. The following software automation tools will be supported:

* Chef
* Ansible

The following built-in automation will not be supported:

* Apache
* Tomcat
* Nginx
* HAProxy
* MySQL
* Percona
* MariaDB
* RabbitMQ
* Redis
* Memcached

Users can still install the platforms above using orchestration scripts or our integration with configuration tools, but it will no longer be included in Scalr built-in automation.

Ubuntu 12.04 Support
--------------------

Ubuntu 12.04 will no longer be supported by the latest Scalarizr versions. We have made some improvements to our APT repository so that each Ubuntu/Debian OS version has its own Scalarizr package. Scalarizr 6.5.2 will be the last version to support Ubuntu 12.04 or less.
