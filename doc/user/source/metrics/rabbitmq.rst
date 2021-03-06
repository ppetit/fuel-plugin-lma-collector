RabbitMQ metrics
----------------
.. _rabbitmq_metrics:

A collection of RabbitMQ metrics.

* ``rabbitmq_connections``, the total number of connections.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_consumers``, the total number of consumers.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_channels``, the total number of channels.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_exchanges``, the total number of exchanges.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_messages``, the total number of messages which are ready to be
  consumed or not yet acknowledged.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_queues``, the total number of queues.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_running_nodes``, the total number of running nodes in the cluster.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_disk_free``, the free disk space.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_disk_free_limit``, the minimum amount of free disk space for
  RabbitMQ. When ``rabbitmq_disk_free`` drops below this value, all producers
  are blocked.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_remaining_disk``, the difference between ``rabbitmq_disk_free``
  and ``rabbitmq_disk_free_limit``.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_used_memory``, bytes of memory used by the whole RabbitMQ process.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_vm_memory_limit``, the maximum amount of memory allocated for
  RabbitMQ. When ``rabbitmq_used_memory`` uses more than this value, all
  producers are blocked.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``rabbitmq_remaining_memory``, the difference between
  ``rabbitmq_vm_memory_limit`` and ``rabbitmq_used_memory``.

RabbitMQ checks
^^^^^^^^^^^^^^^
.. _rabbitmq_checks:

* ``rabbitmq_check``, check the availability status of the ``rabbitmq`` service
  on a node. The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.
