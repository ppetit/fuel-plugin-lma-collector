AFD and GSE metrics
^^^^^^^^^^^^^^^^^^^
.. _afd_gse_metrics:

The AFD and GSE metrics are health status metrics created by the
operational insight pipeline of StackLight.

The GSE (Global Status Evaluation) metrics are health status metrics that apply to the clusters.
The AFD (Anomaly and Fault Detection) metrics are derived from the execution of alarms. 

For details about the GSE and AFD metrics, see :ref:`Configuring alarms <configure_alarms>`.

.. todo: Fix the the <configure_alarms> reference.

* ``cluster_status``, the health status of a cluster. A cluster can be a service
  cluster (i.e. Nova scheduler cluster), a node cluster (i.e. controller cluster,
  or a top-level cluster (i.e Nova control plane).

  The supported values for the ``status`` metric is one of:

  - ``0`` for the *Okay* status.
  - ``1`` for the *Warning* status.
  - ``2`` for the *Unknown* status.
  - ``3`` for the *Critical* status.
  - ``4`` for the *Down* status.

  Dimensions:

  - cluster_name, the name of the cluster if ``cluster_status``
    is for a ``top-level`` cluster.
  - member, contains always the name of the cluster irrespective of the
    type of cluster.
  - nagios_host: identifies the virtual hostname where ``cluster_status``
    is displayed in the Nagios UI.
  - service: if ``cluster_status`` is about a service cluster,
    then ``service`` contains the name of the cluster.

|

* ``status``, the health status of a monitored entity derived from the
  execution of an alarm.

  The supported values for the ``status`` metric is one of:

  - ``0`` for the *Okay* status.
  - ``1`` for the *Warning* status.
  - ``2`` for the *Unknown* status.
  - ``3`` for the *Critical* status.
  - ``4`` for the *Down* status.

  Dimensions:

  - ``backend``, the name of the HAProxy backend the alarm applies to (optional).
  - ``hostname``, the hostname the alarm applies to.
  - ``member``, the name of the alarm.
  - ``node_role``, the role of the node the alarm applies to (optional).
  - ``process``, the name of the process the alarm applies to (optional).
  - ``service``, the name of the service the alarm applies to (optional).