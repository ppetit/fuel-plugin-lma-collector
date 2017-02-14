.. _metrics:

The StackLight Metrics
----------------------

In this chapter you will find a list of all the metrics collected by StackLight.

The actual amount of metrics increases regularly from one release of StackLight to next
as more measurements and checks are performed. In the current 1.0 version, that number
approaches *700 different metrics* and many more times-series.

The metrics are stored in InfluxDB as ``measurements``.
In StackLight, the value of a metric is always stored in a 'value' ``field key`` while
the 'dimensions' (metric metadata) are stored in one or several ``tag keys``.
The dimensions (``tag keys``) are indexed by InfluxDB while the values
(``field keys``) are not. Also, in StackLight all the values are numbers (float),
and all the metrics have an ``environment_label`` dimension which will not be repeated
hereafter. The ``environment_label`` dimension can be useful to aggregate metrics
coming from multiple MCP deployment sources.

System metrics
++++++++++++++

.. include:: metrics/system.rst

Apache metrics
++++++++++++++

.. include:: metrics/apache.rst

Nginx metrics
+++++++++++++

../include:: metrics/nginx.rst

MySQL metrics
+++++++++++++

.. include:: metrics/mysql.rst

RabbitMQ metrics
++++++++++++++++

.. include:: metrics/rabbitmq.rst

HAProxy metrics
+++++++++++++++

.. include:: metrics/haproxy.rst

Pacemaker metrics
+++++++++++++++++

.. include:: metrics/pacemaker.rst

Memcached metrics
+++++++++++++++++

.. include:: metrics/memcached.rst

Libvirt metrics
+++++++++++++++

.. include:: metrics/libvirt.rst

GlusterFS metrics
+++++++++++++++++

.. include:: metrics/glusterfs.rst

OpenStack metrics
+++++++++++++++++

.. include:: metrics/openstack.rst

OpenContrail metrics
++++++++++++++++++++

.. include:: metrics/opencontrail.rst

Ceph metrics
++++++++++++

.. include:: metrics/ceph.rst

Cluster  metrics
++++++++++++++++

.. include:: metrics/clusters.rst

Self-monitoring metrics
+++++++++++++++++++++++

.. include:: metrics/lma.rst

Elasticsearch metrics
+++++++++++++++++++++

.. include:: metrics/elasticsearch.rst

InfluxDB metrics
++++++++++++++++

.. include:: metrics/influxdb.rst
