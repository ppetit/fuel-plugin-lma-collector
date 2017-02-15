Memcached metrics
^^^^^^^^^^^^^^^^^
.. _memcached_metrics:

A collection of Memcached metrics. For additional details about these
metrics, see the `Memcached documentation <https://github.com/memcached/memcached/blob/master/doc/protocol.txt#L488>`_.

* ``memcached_command_flush``, the cumulative number of flush reqs.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``memcached_command_get``, the cumulative number of retrieval reqs.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
 
|
 
* ``memcached_command_set``, the cumulative number of storage reqs.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_command_touch``, the cumulative number of touch reqs.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_connections_current``, the number of open connections.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_df_cache_free``, the current number of free bytes to store items.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
 
|
 
* ``memcached_df_cache_used``, the current number of bytes used to store items.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_items_current``, the current number of items stored.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_octets_rx``, the total number of bytes read by this server from
  the network.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_octets_tx``, the total number of bytes sent by this server to
  the network.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ops_decr_hits``, the number of successful decr reqs.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ops_decr_misses``, the number of decr reqs against missing keys.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ops_evictions``, the number of valid items removed from cache to
  free memory for new items.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ops_hits``, the number of keys that have been requested.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ops_incr_hits``, the number of successful incr reqs.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ops_incr_misses``, the number of successful incr reqs.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ops_misses``, the number of items that have been requested and
  not found.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_percent_hitratio``, the percentage of get command hits (in cache).

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ps_cputime_syst``, the percentage of CPU time spent in system
  mode by memcached. It can be greater than 100% when the node has more than
  one CPU.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
|

* ``memcached_ps_cputime_user``, the percentage of CPU time spent in user mode
  by memcached. It can be greater than 100% when the node has more than one CPU.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  
Memcached checks
^^^^^^^^^^^^^^^^
.. _memcached_checks:

* ``memcached_check``, check the availability status of the Memcached service or process
  on a node. The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.