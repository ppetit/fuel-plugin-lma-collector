GlusterFS metrics
^^^^^^^^^^^^^^^^^
.. _glusterfs_metrics:

A collection of GlusterFS metrics.

GlusterFS checks
^^^^^^^^^^^^^^^^^^^^
.. _glusterfs_checks:

* ``glusterfs_check``, check the availability of the GlusterFS service on a node.
  The value of the metric is ``1`` if the check is successful or ``0`` if not successful.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.

GlusterFS metrics
^^^^^^^^^^^^^^^^^

The GlusterFS metrics are collected locally from all the controller nodes.
Therefore, based on the current implementation, the ``hostname`` dimension doesn't
always reflect the hostname the metric applies to but rather where it is collected from.
In those cases, you should instead use to the ``peer`` dimension to get the hostname
the metric applies to.

* ``glusterfs_inodes_free``, the number of free inodes.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the GlusterFS volume.

|

* ``glusterfs_inodes_percent_free``, the percentage of free inodes.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from..
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the GlusterFS volume.

|

* ``glusterfs_inodes_percent_used``, the percentage of used inodes.
  
  Dimensions:
  
  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the GlusterFS volume.

|

* ``glusterfs_inodes_used``,  the number of used inodes.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the GlusterFS volume.

|

* ``glusterfs_peer_state``, the GlusterFS peer state where a value:

  - ``0`` represents ``down``.
  - ``1`` represents ``up``.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.

|

* ``glusterfs_peers_count``, the number of GlusterFS peers by state.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``state``, the state of the GlusterFS peer  where ``0`` represents
    ``down`` and ``1`` represents ``up``.

|

* ``glusterfs_peers_percent``, the percent of GlusterFS peers by state.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``state``, the state of the GlusterFS peer where ``0`` represents
    ``down`` and ``1`` represents ``up``.

|

* ``glusterfs_space_free``, the amount of free space in bytes.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the the GlusterFS volume.

|

* ``glusterfs_space_used``, the amount of used space in bytes.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the the GlusterFS volume.  

|

* ``glusterfs_space_percent_free``, the percentage of free space in bytes.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the GlusterFS volume.

|

* ``glusterfs_space_percent_used``, the percentage of used space in bytes.
  
  Dimensions:

  - ``hostname``, the hostname the metric is collected from.
  - ``peer``, the hostname (or IP address) of the GlusterFS peer the metric applies to.
  - ``volume``, the name of the the GlusterFS volume.