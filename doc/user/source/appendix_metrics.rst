.. _metrics:

List of metrics
---------------

Here is a list of all the metrics (with their dimensions) that are collected
by StackLight. In the current version of Stacklight there are 668 differents
metrics. In InfluxDB, the metics are known as ``measurements`` and the dimensions
as ``tag keys``. All the StackLight metrics are decorated with the ``environment_label``
dimension which will not be repeated hereafter. It is a usefull dimension to
identify in which MCP environment a metric was collected.

System
++++++

.. include:: metrics/system.rst

Apache
++++++

.. include:: metrics/apache.rst

MySQL
+++++

.. include:: metrics/mysql.rst

RabbitMQ
++++++++

.. include:: metrics/rabbitmq.rst

HAProxy
+++++++

.. include:: metrics/haproxy.rst

Memcached
+++++++++

.. include:: metrics/memcached.rst

Libvirt
+++++++

.. include:: metrics/libvirt.rst


OpenStack
+++++++++

.. include:: metrics/openstack.rst


Ceph
++++

.. include:: metrics/ceph.rst

Pacemaker
+++++++++

.. include:: metrics/pacemaker.rst

Clusters
++++++++

.. include:: metrics/clusters.rst

Self-monitoring
+++++++++++++++

.. include:: metrics/lma.rst


Elasticsearch
+++++++++++++

.. include:: metrics/elasticsearch.rst


InfluxDB
++++++++

.. include:: metrics/influxdb.rst

Checks
++++++

.. include:: metrics/checks.rst
