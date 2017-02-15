Open Contrail metrics
^^^^^^^^^^^^^^^^^^^^^
.. _opencontrail_metrics:

A collection of OpenContrail related metrics.

Cassandra metrics
^^^^^^^^^^^^^^^^^

The following list of Cassandra metrics retrieved via JMX from the Cassandra services.

For more detailed about these metrics, see the documentation.

Cassandra specific:

- https://wiki.apache.org/cassandra/Metrics
- https://wiki.apache.org/cassandra/JmxInterface
- https://cassandra-zone.com/performance-monitoring
- https://www.datadoghq.com/blog/how-to-collect-cassandra-metrics
- http://batey.info/cassandra-clientrequest-metrics.html

Java specific:

- https://www.dynatrace.com/resources/ebooks/javabook/analyzing-java-memory
- https://plumbr.eu/handbook/gc-tuning-measuring/jmx-api

* ``GenericJMX_cassandra_CMSOldGen``, the size of JVM pool of objects which survived
  after garbage collection from Young Generation.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_CMSPermGen``, the size of JVM pool of objects containing
  permanent class metadata and descriptors information.

  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_CompactionCompletedTasks``, the number of background compaction tasks completed.

  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_CompactionPendingTasks``, the number of background compaction tasks currently in progress.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_DownEndpointCount``, the number of Cassandra nodes in ``down``
  state.
  
  Dimensions:
 
  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_GarbageCollectorCollectionCounta``, the total number of times the GC has run.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_GarbageCollectorCollectionTime``, the accumulated duration of the GC running time in ms.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_StorageDBLoad``, the size of the Casandra database in bytes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_StorageExceptionCount``, the total number of storage exceptions.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_UpEndpointCount``, the number of Cassandra nodes in Up state.

	Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_clientRequest_Read_50thPercentile``, the 50 percentile client requests read latency in ms.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_clientRequest_Read_Mean``, the mean client requests read latency in ms.  

  Dimensions:

 - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_clientRequest_Read_MeanRate``, the mean client requests read throughput.
  
  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_clientRequest_Write_50thPercentile``, the 50 percental client requests write latency in ms.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_clientRequest_Write_Mean``, the mean client requests write latency in ms.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_clientRequest_Write_MeanRate``, the mean client requests write throughput.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_connectedNativeClients``, the number of connected native clients.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_connectedThriftClients``, the number of connected thrift clients.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_memory``, the size of Cassandra JVM heap memory in bytes.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``GenericJMX_cassandra_memory_heap_usage_max``, the maximum size of the Cassandra
  JVM heap memory in bytes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

Contrail BGP metrics
^^^^^^^^^^^^^^^^^^^^
.. _contrail_bgp_metrics:


* ``contrail_bgp_session_count``, the total number of BGP sessions.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_bgp_session_down_count``, the total number of BGP sessions in ``down`` state.
     
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_bgp_session_up_count``, the total number of BGP sessions in ``up`` state.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_ifmap_elements_count`` total number of entries configured in IFMAP. 
        
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_dns_xmpp``, the total number of agent DNS subscription status
  requests.
  
  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_active``, the total number of active flows.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_aged``, the total number of aged flows.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_composite_invalid_interface``, the total number of
  invalid interface errors.  
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_created``, the total number of created flows.
        
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_discard``, the total number of packets going to
  discard nexthop.
        
  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_flow_action_drop``, the total number of flow
  actions drop.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_flow_queue_limit_exceeded``, the number
  of times more than 3 packets are received before flow processing is complete.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_flow_table_full``, the total number of times
  the flow table was full.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_frag_err``, the total number of times enqueueing
  to fragment queue failed.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_invalid_label``, the total number of times a label
  received in the packet was invalid.
        
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_flows_invalid_nh``, the total number of times a
  nexthop was invalid.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_lls``, the total number of HTTP requests to the link
   local address. 
        
  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_vrouter_xmpp``, the total number of XMPP connection status
  requests.
      
  Dimensions:
  
  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_xmpp_session_count``, the total number of XMPP sessions.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_xmpp_session_down_count``, the total number of XMPP sessions in
  ``down`` state.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``contrail_xmpp_session_up_count``, the total number of XMPP sessions in
  ``up`` state.
        
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

Contrail checks
^^^^^^^^^^^^^^^
  .. _contrail_checks:

* ``contrail_check``, check the availability of the Contrail server API endpoint.
  The value of the metric is ``1`` if the check is successful or ``0`` if the check is not successful.
      
  Dimensions:

  - ``hostname``, the hostname the metric applies to.  