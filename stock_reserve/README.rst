=================
Stock Reservation
=================

.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fstock--logistics--warehouse-lightgray.png?logo=github
    :target: https://github.com/OCA/stock-logistics-warehouse/tree/16.0/stock_reserve
    :alt: OCA/stock-logistics-warehouse
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/stock-logistics-warehouse-16-0/stock-logistics-warehouse-16-0-stock_reserve
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runbot-Try%20me-875A7B.png
    :target: https://runbot.odoo-community.org/runbot/153/16.0
    :alt: Try me on Runbot

|badge1| |badge2| |badge3| |badge4| |badge5| 

Allows to create stock reservations on products.

Each reservation can have a validity date, once passed, the reservation
is automatically lifted.

The reserved products are substracted from the virtual stock. It means
that if you reserved a quantity of products which bring the virtual
stock below the minimum, the orderpoint will be triggered and new
purchase orders will be generated. It also implies that the max may be
exceeded if the reservations are canceled.

If ownership of stock is active in the stock settings, you can specify the
owner on the reservation.

**Table of contents**

.. contents::
   :local:

Usage
=====

To make a stock reservation:

#. Go to *Inventory > Products*.
#. Select or create one product with stock.
#. Click on *Stock Reservations* smart button.
#. Create one reservation.
#. Press the button *Reserve*.

You can release a reservation by clicking on the button *Release*

Known issues / Roadmap
======================

* Review multicompany. Take a look of [this](https://github.com/OCA/stock-logistics-warehouse/pull/1346) PR

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/stock-logistics-warehouse/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed
`feedback <https://github.com/OCA/stock-logistics-warehouse/issues/new?body=module:%20stock_reserve%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Camptocamp

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/stock-logistics-warehouse <https://github.com/OCA/stock-logistics-warehouse/tree/16.0/stock_reserve>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
