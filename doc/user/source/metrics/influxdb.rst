InfluxDB metrics
----------------
.. _influxdb_metrics:

InfluxDB cluster metrics
^^^^^^^^^^^^^^^^^^^^^^^^
.. _influxdb_cluster_metrics:

The InfluxDB cluster metrics are global metrics available only when the InfluxDB
is installed in cluster mode.

* ``influxdb_cluster_write_shard_points_requests``, the number of requests for
  writing a time series points to a shard.

* ``influxdb_cluster_write_shard_requests``, the number of requests for writing
  to a shard.

InfluxDB HTTP metrics
^^^^^^^^^^^^^^^^^^^^^
.. _influxdb_http_metrics:

* ``influxdb_httpd_failed_auths``, the number of failed authentications.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_httpd_ping_requests``, the number of ping requests.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_httpd_query_requests``, the number of query requests received.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_httpd_query_response_bytes``, the number of bytes returned to the
  client.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_httpd_requests``, the number of requests received.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_httpd_write_points_ok``, the number of points successfully written.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_httpd_write_request_bytes``, the number of bytes received for
  write requests.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_httpd_write_requests``, the number of write requests received.

  dimensions:

  - hostname, the hostname the metric applies to.

InfluxDB write metrics
^^^^^^^^^^^^^^^^^^^^^^
.. _influxdb_write_metrics:

* ``influxdb_write_local_point_requests``, the number of write points requests
  from the local data node.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_write_ok``, the number of successful writes of consistency level.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_write_point_requests``, the number of write points requests across
  all data nodes.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_write_remote_point_requests``, the number of write points requests
  to remote data nodes.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_write_requests``, the number of write requests across all data
  nodes.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_write_sub_ok``, the number of successful points sent to
  subscriptions.

  dimensions:

  - hostname, the hostname the metric applies to.

InfluxDB Runtime metrics
^^^^^^^^^^^^^^^^^^^^^^^^
.. _influxdb_runtime_metrics:

* ``influxdb_garbage_collections``, the number of garbage collections.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_go_routines``, the number of Golang routines.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_heap_idle``, the number of bytes in idle spans.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_heap_in_use``, the number of bytes in non-idle spans.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_heap_objects``, the total number of allocated objects.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_heap_released``, the number of bytes released to the operating
  system.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_heap_system``, the number of bytes obtained from the system.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_memory_alloc``, the number of bytes allocated and not yet freed.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_memory_frees``, the number of free operations.


  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_memory_lookups``, the number of pointer lookups.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_memory_mallocs``, the number of malloc operations.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_memory_system``, the number of bytes obtained from the system.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``influxdb_memory_total_alloc``, the number of bytes allocated (even if freed).

  dimensions:

  - hostname, the hostname the metric applies to.

InfluxDB checks
^^^^^^^^^^^^^^^
.. _influxdb_checks:

* ``influxdb_check``, check the availability status of the Influxdb service.
  The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.

  dimensions:
  
  - hostname, the hostname the metric applies to.

The following metrics are generated using the output of the :command:``show stats``
command. The value of these metrics are reset to zero when InfluxDB is restarted.
