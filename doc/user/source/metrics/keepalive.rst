Keepalive metrics
^^^^^^^^^^^^^^^^^
.. _keepalive_metrics:

A collection of Keepalive related metrics.

* ``vrrp``, A Virtual Router Redundancy Protocol (VRRP) metric.
  The value of the metric is ``1`` if the VIP is active on the node or
  ``0`` if the VIP is not active.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``ip_address``, the IP address of the VIP
  - ``label``, the name of the VIP as defined in the reclass model.
