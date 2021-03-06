..
      Copyright 2012 New Dream Network (DreamHost)

      Licensed under the Apache License, Version 2.0 (the "License"); you may
      not use this file except in compliance with the License. You may obtain
      a copy of the License at

          http://www.apache.org/licenses/LICENSE-2.0

      Unless required by applicable law or agreed to in writing, software
      distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
      WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
      License for the specific language governing permissions and limitations
      under the License.

.. _measurements:

==============
 Measurements
==============

Existing meters
===============

For the list of existing metrics see the tables under the
`Measurements page`_ of Ceilometer in the Cloud Administrator Guide.

.. _Measurements page: http://docs.openstack.org/admin-guide-cloud/content/section_telemetry-measurements.html

Adding new meters
=================

If you would like to add new meters please check the
:ref:`add_new_meters` page under in the Contributing
section.

OSprofiler data
===============

All messages with event type "profiler.*" will be collected as profiling data.
Using notification plugin profiler/notifications.py.

.. note::

  Be sparing with heavy usage of OSprofiler, especially in case of complex
  operations like booting and deleting instance that may create over 100kb of
  sample data per each request.
