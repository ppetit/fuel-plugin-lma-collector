.. _elasticsearch_metrics:

Elasticsearch checks
^^^^^^^^^^^^^^^^^^^^
.. _elasticsearch_checks:

* ``elasticsearch_check``, check the availability status of the Elasticsearch service.
  The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.
  
  Dimensions:

  - hostname, the hostname the metric applies to.

Elsticsearch cluster metrics
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. _elasticsearch_cluser_metrics:

The following list of metrics are cluster wide metrics.
They are obtained  through querying the Elasticsearch API.
For details about these metrics,
see the `documentation <https://www.elastic.co/guide/en/elasticsearch/reference/1.7/cluster-health.html>`_.

* ``elasticsearch_cluster_active_primary_shards``, the number of active primary
  shards.

* ``elasticsearch_cluster_active_shards``, the number of active shards.

* ``elasticsearch_cluster_health``, the health status of the Elasticsearch
  cluster as reported by Elasticsearch itself where:

  - value ``1`` represents ``okay`` (green).
  - value ``2`` represents ``warning`` (yellow).
  - value ``3`` represents ``critical`` (red).
  
  Note that a ``critical`` status may also be reported when the
  Elasticsearch API returns an unexpected result like a connection
  error which doesn't necessarily mean that the Elasticsearch server
  itself is critical.

* ``elasticsearch_cluster_initializing_shards``, the number of initializing
  shards.
  
* ``elasticsearch_cluster_number_of_nodes``, the number of nodes in the cluster.

* ``elasticsearch_cluster_number_of_pending_tasks``, the number of pending tasks.

* ``elasticsearch_cluster_relocating_shards``, the number of relocating shards.

* ``elasticsearch_cluster_unassigned_shards``, the number of unassigned shards.
  
* ``elasticsearch_documents``, the number of documents.
  
  In Elasticsearch, a document refers to the top-level,
  or root object that is serialized into JSON and stored
  in Elasticsearch under a unique ID.
  
* ``elasticsearch_documents_deleted``, number of documents deleted.