Libvirt metrics
---------------
.. _libvirt-metrics:

All libvirt metrics contains an ``instance_id`` dimension which contains the
UUID of the Nova instance.

Libvirt CPU metrics
^^^^^^^^^^^^^^^^^^^
.. _libvirt_cpu_metrics:

* ``virt_cpu_time``, the average amount of CPU time (in nanoseconds) allocated
  to the virtual instance within the last second.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.

* ``virt_vcpu_time``, the average amount of CPU time (in nanoseconds)
  allocated to the virtual CPU within the last second.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - vcpu_number, the virtual CPU number.

Libvirt disk metrics
^^^^^^^^^^^^^^^^^^^^
.. _libvirt_disk_metrics:

These metrics have in addition a ``device`` dimension that contains the
name of virtual disk device to which the metric applies.
For example, 'vda', 'vdb', and so forth.

* ``virt_disk_octets_read``, the number of octets (bytes) read per second.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - device, the name of the device the metric applies to.

* ``virt_disk_octets_write``, the number of octets (bytes) written per second.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - device, the name of the device the metric applies to.

* ``virt_disk_ops_read``, the number of read operations per second.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - device, the name of the device the metric applies to.

* ``virt_disk_ops_write``, the number of write operations per second.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - device, the name of the device the metric applies to.

Memory metrics
^^^^^^^^^^^^^^
.. _libvirt_memory_metrics:

* ``virt_memory_total``, the total amount of memory (in bytes) allocated to the
  virtual instance.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.

Network metrics
^^^^^^^^^^^^^^^
.. _libvirt_network_metrics:

There metrics have an ``interface`` dimension that contains
the interface name to which the metric applies.
For example, 'tap0dc043a6-dd', 'tap769b123a-2e', and so forth.

* ``virt_if_dropped_rx``, the number of dropped packets per second when
  receiving from the interface.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

* ``virt_if_dropped_tx``, the number of dropped packets per second when
  transmitting from the interface.

   dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

* ``virt_if_errors_rx``, the number of errors per second detected when
  receiving from the interface.

  dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

* ``virt_if_errors_tx``, the number of errors per second detected when
  transmitting from the interface.

   dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

* ``virt_if_octets_rx``, the number of octets (bytes) received per second by
  the interface.

   dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

* ``virt_if_octets_tx``, the number of octets (bytes) transmitted per second by
  the interface.

   dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

* ``virt_if_packets_rx``, the number of packets received per second by the
  interface.

   dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

* ``virt_if_packets_tx``, the number of packets transmitted per second by the
  interface.

   dimensions:

  - hostname, the hostname the metric applies to.
  - instance_id, the libvirt instance ID.
  - interface, the libvirt network interface name.

libvirt checks
^^^^^^^^^^^^^^
.. _libvirt_checks:

* ``libvirt_check``, check the availability status of the libvirt service
  on a node. The value of the metric is ``1`` if the check is successful or ``0``
  if the check is not successful.
  
  dimensions:

  - hostname, the hostname the metric applies to.
