MySQL metrics
-------------
.. _mysql_metrics:

A collection of MySQL metrics.

Command metrics
^^^^^^^^^^^^^^^

* ``mysql_commands``, the number of times per second a given statement has been
  executed.

  dimensions:

  - hostname, the hostname the metric applies to.
  - statement, the ``statement`` dimension contains the name of the MySQL
    statement that applies to the metric applies.
    It can be one of the following values:

    - ``change_db`` for the USE statement.
    - ``commit`` for the COMMIT statement.
    - ``flush`` for the FLUSH statement.
    - ``insert`` for the INSERT statement.
    - ``rollback`` for the ROLLBACK statement.
    - ``select`` for the SELECT statement.
    - ``set_option`` for the SET statement.
    - ``show_collations`` for the SHOW COLLATION statement.
    - ``show_databases`` for the SHOW DATABASES statement.
    - ``show_fields`` for the SHOW FIELDS statement.
    - ``show_master_status`` for the SHOW MASTER STATUS statement.
    - ``show_status`` for the SHOW STATUS statement.
    - ``show_tables`` for the SHOW TABLES statement.
    - ``show_variables`` for the SHOW VARIABLES statement.
    - ``show_warnings`` for the SHOW WARNINGS statement.
    - ``update`` for the UPDATE statement.

Handler metrics
^^^^^^^^^^^^^^^

* ``mysql_handler``, the number of times per second a given handler has been
  executed.

  dimensions:

  - hostname, the hostname the metric applies to.
  - handler, the ``handler`` dimension contains the name of the MySQL
    handler that applies to the metric.
    It can be one of the following values:

    - ``commit`` for the internal COMMIT statements.
    - ``delete`` for the internal DELETE statements.
    - ``external_lock`` for the external locks.
    - ``read_first`` for the requests that read the first entry in an index.
    - ``read_key`` for the requests that read a row based on a key.
    - ``read_next`` for the requests that read the next row in key order.
    - ``read_prev`` for the requests that read the previous row in key order.
    - ``read_rnd`` for the requests that read a row based on a fixed position.
    - ``read_rnd_next`` for the requests that read the next row in the data file.
    - ``rollback`` the requests that perform the rollback operation.
    - ``update`` the requests that update a row in a table.
    - ``write`` the requests that insert a row in a table.

Locks metrics
^^^^^^^^^^^^^

* ``mysql_locks_immediate``, the number of times per second the requests for
  table locks could be granted immediately.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_locks_waited``, the number of times per second the requests for
  table locks had to wait.

  dimensions:

  - hostname, the hostname the metric applies to.

Network metrics
^^^^^^^^^^^^^^^

* ``mysql_octets_rx``, the number of bytes per second received by the server.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_octets_tx``, the number of bytes per second sent by the server.

  dimensions:

  - hostname, the hostname the metric applies to.

Thread metrics
^^^^^^^^^^^^^^

* ``mysql_threads_cached``, the number of threads in the thread cache.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_threads_connected``, the number of currently open connections.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_threads_created``, the number of threads created per second to
  handle connections.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_threads_running``, the number of threads that are not sleeping.

  dimensions:

  - hostname, the hostname the metric applies to.

Cluster metrics
^^^^^^^^^^^^^^^

The following metrics are collected with statement 'SHOW STATUS'. For details,
see the `Percona documentation <http://www.percona.com/doc/percona-xtradb-cluster/5.6/wsrep-status-index.html>`_.

* ``mysql_cluster_connected``, Has for value ``1`` when the node is connected
  to the cluster, if not, then ``0``.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_local_cert_failures``, the number of write sets that failed
  the certification test.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_local_commits``, the number of write sets committed on the
  node.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_local_recv_queue``, the number of write sets waiting to be
  applied.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_local_send_queue``, the number of write sets waiting to be
  sent.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_ready``, ``1`` when the node is ready to accept queries, if
  not, then ``0``.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_received``, the total number of write sets received from
  other nodes.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_received_bytes``, the total size in bytes of write sets
  received from other nodes.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_replicated``, the total number of write sets sent to other
  nodes.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_replicated_bytes`` the total size in bytes of write sets sent
  to other nodes.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_size``, the current number of nodes in the cluster.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``mysql_cluster_status``, ``1`` when the node is 'Primary', ``2`` if
  'Non-Primary', and ``3`` if 'Disconnected'.

  dimensions:

  - hostname, the hostname the metric applies to.

Slow queries
^^^^^^^^^^^^

The ``mysql_slow_queries`` metric is obtained from the statement
'SHOW STATUS where Variable_name = 'Slow_queries'.

* ``mysql_slow_queries``, the number of queries that have taken more than X
  seconds, depending on the MySQL configuration parameter 'long_query_time'
  (10s per default).

MySQL checks
^^^^^^^^^^^^
.. _mysql_checks:

* ``mysql_check``, check the availability status of the ``mysql`` service or process
  on a node. The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.

  dimensions:

  - hostname, the hostname the metric applies to.
