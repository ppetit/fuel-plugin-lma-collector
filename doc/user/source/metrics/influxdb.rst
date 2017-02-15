InfluxDB metrics
^^^^^^^^^^^^^^^^
.. _influxdb_metrics:

A collection of InfluxDB metrics.

InfluxDB cluster metrics
^^^^^^^^^^^^^^^^^^^^^^^^

The InfluxDB cluster metrics are global metrics available only when the InfluxDB
is installed in cluster mode.

* ``influxdb_cluster_write_shard_points_requests``, the number of requests for
  writing a time-series data-points to a shard.

|

* ``influxdb_cluster_write_shard_requests``, the number of requests for writing
  to a shard.

InfluxDB HTTP metrics
^^^^^^^^^^^^^^^^^^^^^

* ``influxdb_httpd_failed_auths``, the number of failed authentications.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_httpd_ping_requests``, the number of ping requests.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_httpd_query_requests``, the number of query requests received.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_httpd_query_response_bytes``, the number of bytes returned to the
  client.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_httpd_requests``, the number of requests received.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_httpd_write_points_ok``, the number of points successfully written.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_httpd_write_request_bytes``, the number of bytes received for
  write requests.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_httpd_write_requests``, the number of write requests received.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

InfluxDB write metrics
^^^^^^^^^^^^^^^^^^^^^^

* ``influxdb_write_local_point_requests``, the number of write points requests
  from the local data node.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_write_ok``, the number of successful writes of consistency level.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_write_point_requests``, the number of write points requests across
  all data nodes.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_write_remote_point_requests``, the number of write points requests
  to remote data nodes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_write_requests``, the number of write requests across all data
  nodes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_write_sub_ok``, the number of successful points sent to
  subscriptions.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

InfluxDB runtime metrics
^^^^^^^^^^^^^^^^^^^^^^^^

* ``influxdb_garbage_collections``, the number of garbage collections.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_go_routines``, the number of Golang routines.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_heap_idle``, the number of bytes in idle spans.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_heap_in_use``, the number of bytes in non-idle spans.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_heap_objects``, the total number of allocated objects.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_heap_released``, the number of bytes released to the operating
  system.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_heap_system``, the number of bytes obtained from the system.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_memory_alloc``, the number of bytes allocated and not yet freed.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_memory_frees``, the number of free operations.


  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_memory_lookups``, the number of pointer lookups.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_memory_mallocs``, the number of malloc operations.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_memory_system``, the number of bytes obtained from the system.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``influxdb_memory_total_alloc``, the number of bytes allocated (even if freed).

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

InfluxDB checks
^^^^^^^^^^^^^^^
.. _influxdb_checks:

* ``influxdb_check``, check the availability status of the Influxdb service.
  The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.

  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

The following metrics are generated using the output of the :command:``show stats``
command. The value of these metrics are reset to zero when InfluxDB is restarted.
