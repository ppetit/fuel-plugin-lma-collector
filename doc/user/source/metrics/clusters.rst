.. _cluster_metrics:

Cluster metrics
^^^^^^^^^^^^^^^

The cluster metrics are known as the GSE metrics.
They are emitted by the Aggregator.
For details about the GSE metrics, see
:ref:`Configuring alarms <configure_alarms>`.

TODO: Fix the the reference above

* ``cluster_status``, the status of a cluster. A cluster can be a service
  cluster (i.e. Nova scheduler cluster), a node cluster (i.e. controller cluster,
  or a top-level cluster (i.e Nova control plane).

  Dimensions:

  - cluster_name: if ``cluster_status`` is about a top-level cluster,
    then ``cluster_name`` contains the name of the cluster.
  - environment_label: the environment name the metric was collected from.
  - member: contains the name of the cluster ``cluster_status`` applies to.
  - nagios_host: identifies the virtual hostname where ``cluster_status``
    is displayed in the Nagios UI.
  - service: if ``cluster_status`` is about a service cluster,
    then ``service`` contains the name of the cluster.

  The supported values for the ``cluster_status`` metric are:

  - ``0`` for the *Okay* status.

  - ``1`` for the *Warning* status.

  - ``2`` for the *Unknown* status.

  - ``3`` for the *Critical* status.

  - ``4`` for the *Down* status.