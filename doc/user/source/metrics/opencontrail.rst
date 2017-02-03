.. _opencontrail_metrics:

Cassandra metrics
^^^^^^^^^^^^^^^^^
.. _cassandra_metrics:

The following list of Cassandra metrics retrieved via JMX from the Cassandra services.

For more detailed about these metrics, see the documentation.

Cassandra specific:

- <https://wiki.apache.org/cassandra/Metrics>`_
- <https://wiki.apache.org/cassandra/JmxInterface>`_
- <https://cassandra-zone.com/performance-monitoring/`>`_
- <https://www.datadoghq.com/blog/how-to-collect-cassandra-metrics/>_`
- <http://batey.info/cassandra-clientrequest-metrics.html>_`

Java specific:

- <https://www.dynatrace.com/resources/ebooks/javabook/analyzing-java-memory>`_
- <https://plumbr.eu/handbook/gc-tuning-measuring/jmx-api>`_

* ``GenericJMX_cassandra_CMSOldGen``, the size of JVM pool of objects which survived
  after garbage collection from Young Generation.

  Dimensions:
  
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_CMSPermGen``, the size of JVM pool of objects containing
  permanent class metadata and descriptors information.

   Dimensions:
  
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_CompactionCompletedTasks``, the number of background compaction tasks completed.

  Dimensions:
  
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_CompactionPendingTasks``, the number of background compaction tasks currently in progress.

  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_DownEndpointCount``, the number of Cassandra nodes in Down state.
  
  Dimensions:
 
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_GarbageCollectorCollectionCounta``, the total number of times the GC has run.

  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_GarbageCollectorCollectionTime``, the accumulated duration of the GC running time in ms.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_StorageDBLoad``, the size of Casandra database in bytes.

  Desciption:
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_StorageExceptionCount``, the total number of storage exceptions.

  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_UpEndpointCount``, the number of Cassandra nodes in Up state.

	Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_clientRequest_Read_50thPercentile``, the 50 percental client requests read latency in ms.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_clientRequest_Read_Mean``, the mean client requests read latency in ms.  

  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_clientRequest_Read_MeanRate``,  the mean client requests read throughput.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_clientRequest_Write_50thPercentile``, the 50 percental client requests write latency in ms.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_clientRequest_Write_Mean``, the mean client requests write latency in ms.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_clientRequest_Write_MeanRate``, the mean client requests write throughput.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_connectedNativeClients``, the number of connected native clients.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_connectedThriftClients``, the number of connected thrift clients.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_memory``, the size of Cassandra JVM heap memory in bytes.
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``GenericJMX_cassandra_memory_heap_usage_max``, the maximum size of the Cassandra
  JVM heap memory in bytes.

  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

Contrail BGP
^^^^^^^^^^^^
.. _contrail_bgp_metrics:

* ``contrail_bgp_session_count``
   
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_bgp_session_down_count``
     
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_bgp_session_up_count``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_check``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_ifmap_elements_count``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_dns_xmpp``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_active``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_aged``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_composite_invalid_interface``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_created``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_discard``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_flow_action_drop``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_flow_queue_limit_exceeded``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_flow_table_full``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_frag_err``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_invalid_label``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_flows_invalid_nh``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_lls``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_vrouter_xmpp``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_xmpp_session_count``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_xmpp_session_down_count``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

* ``contrail_xmpp_session_up_count``
      
  
  
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.



fs_inodes_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_inodes_percent_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_inodes_percent_reserved
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_inodes_percent_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_inodes_reserved
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_inodes_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_space_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_space_percent_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_space_percent_reserved
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_space_percent_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_space_reserved
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

fs_space_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
fs
  - hostname, the hostname the metric applies to.

glusterfs_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

glusterfs_inodes_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

glusterfs_inodes_percent_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

glusterfs_inodes_percent_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

glusterfs_inodes_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

glusterfs_peer_state
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer

glusterfs_peers_count``
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

glusterfs_peers_percent
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

glusterfs_space_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

glusterfs_space_percent_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

glusterfs_space_percent_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

glusterfs_space_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
peer
volume

haproxy_backend_bytes_in
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_bytes_out
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_denied_requests
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_denied_responses
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_downtime
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_error_connection
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_error_responses
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_queue_current
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_redistributed
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_response_1xx
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_response_2xx
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_response_3xx
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_response_4xx
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_response_5xx
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_response_other
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_retries
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_server
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
server
state

haproxy_backend_servers
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

haproxy_backend_servers_percent
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

haproxy_backend_session_current
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_session_total
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_backend_status
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_connections
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_frontend_bytes_in
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_bytes_out
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_denied_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_denied_responses
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_error_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_response_1xx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_response_2xx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_response_3xx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_response_4xx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_response_5xx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_response_other
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_session_current
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_frontend_session_total
  Dimensions:

  - environment_label, the environment name the metric was collected from.
frontend
  - hostname, the hostname the metric applies to.

haproxy_pipes_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_pipes_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_run_queue
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_ssl_connections
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_tasks
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

haproxy_uptime
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

hdd_errors_rate
  Dimensions:

  - device
  - environment_label, the environment name the metric was collected from.

http_check_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.

if_collisions
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_dropped_rx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_dropped_tx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_rx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_rx_crc
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_rx_fifo
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_rx_frame
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_rx_length
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_rx_missed
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_rx_over
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_tx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_tx_aborted
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_tx_carrier
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_tx_fifo
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_tx_heartbeat
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_errors_tx_window
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_multicast
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_octets_rx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_octets_tx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_packets_rx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

if_packets_tx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
interface

influxdb_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_garbage_collections
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_go_routines
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_heap_idle
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_heap_in_use
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_heap_objects
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_heap_released
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_heap_system
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_failed_auths
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_ping_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_query_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_query_response_bytes
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_write_points_ok
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_write_request_bytes
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_httpd_write_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_memory_alloc
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_memory_frees
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_memory_lookups
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_memory_mallocs
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_memory_system
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_memory_total_alloc
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_write_ok
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_write_point_local_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_write_point_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_write_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

influxdb_write_sub_ok
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

libvirt_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

lma_components_cputime_syst
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_cputime_user
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_disk_bytes_read
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_disk_bytes_write
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_disk_ops_read
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_disk_ops_write
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_memory_code
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_memory_data
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_memory_rss
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_memory_virtual
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_pagefaults_majflt
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_pagefaults_minflt
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_processes
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_stacksize
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

lma_components_threads
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

load_longterm
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

load_midterm
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

load_shortterm
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

log_messages
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
level
service

logged_users
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_command_flush
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_command_get
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_command_set
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_command_touch
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_connections_current
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_df_cache_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_df_cache_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_items_current
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_octets_rx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_octets_tx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ops_decr_hits
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ops_decr_misses
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ops_evictions
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ops_hits
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ops_incr_hits
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ops_incr_misses
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ops_misses
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_percent_hitratio
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ps_cputime_syst
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memcached_ps_cputime_user
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memory_buffered
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memory_cached
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memory_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memory_slab_recl
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memory_slab_unrecl
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

memory_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_connected
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_local_cert_failures
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_local_commits
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_local_send_queue
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_ready
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_received
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_received_bytes
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_replicated
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_replicated_bytes
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_size
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_cluster_status
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_commands
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
statement

mysql_handler
  Dimensions:

  - environment_label, the environment name the metric was collected from.
handler
  - hostname, the hostname the metric applies to.

mysql_locks_immediate
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_locks_waited
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_octets_rx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_octets_tx
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_slow_queries
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_threads_cached
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_threads_connected
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

mysql_threads_running
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_connections_accepted
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_connections_active
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_connections_handled
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_connections_reading
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_connections_waiting
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_connections_writing
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

nginx_requests
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

ntp_frequency_offset_loop
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

ntp_time_dispersion_peer
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
server

ntp_time_offset_error
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

ntp_time_offset_loop
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

ntp_time_offset_peer
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
server

openstack_check_api
  Dimensions:

  - environment_label, the environment name the metric was collected from.
service

openstack_check_local_api
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service

openstack_cinder_http_response_times
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
http_method
http_status

openstack_cinder_service
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service
state

openstack_cinder_services
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service
state

openstack_cinder_services_percent
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service
state

openstack_glance_http_response_times
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
http_method
http_status

openstack_heat_http_response_times
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
http_method
http_status

openstack_keystone_http_response_times
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
http_method
http_status

openstack_keystone_roles
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_keystone_tenants
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

openstack_keystone_users
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

openstack_neutron_http_response_times
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
http_method
http_status

openstack_neutron_networks
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

openstack_neutron_subnets
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_free_disk
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_free_ram
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_free_vcpus
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_http_response_times
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
http_method
http_status

openstack_nova_running_instances
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_running_tasks
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_service
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service
state

openstack_nova_services
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service
state

openstack_nova_services_percent
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
service
state

openstack_nova_total_free_disk
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_total_free_ram
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_total_free_vcpus
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_total_running_instances
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_total_running_tasks
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_total_used_disk
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_total_used_ram
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_total_used_vcpus
  Dimensions:

  - environment_label, the environment name the metric was collected from.

openstack_nova_used_disk
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_used_ram
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

openstack_nova_used_vcpus
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

pending_operations
  Dimensions:

  - device
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

processes_count``
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
state

processes_fork_rate
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_channels
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_connections
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_consumers
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_disk_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_disk_free_limit
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_exchanges
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_messages
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_queues
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_remaining_disk
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_remaining_memory
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_running_nodes
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_used_memory
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

rabbitmq_vm_memory_limit
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

status
  Dimensions:

backend
  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
member
node_role
process
service

swap_cached
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

swap_free
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

swap_io_in
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

swap_io_out
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

swap_percent_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

swap_used
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

total_threads_created
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

uptime
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

vrrp
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.
ip_address
label

vrrp_check
  Dimensions:

  - environment_label, the environment name the metric was collected from.
  - hostname, the hostname the metric applies to.

