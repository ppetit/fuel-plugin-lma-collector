OpenStack metrics
^^^^^^^^^^^^^^^^^^^^^
.. _openstack_metrics:

A collection of OpenStack metrics.

API check metrics
^^^^^^^^^^^^^^^^^
.. _openstack_api_check_metrics:

* ``openstack_check_api``, the OpenStack service API status
  checked through the load balancer VIP.
  The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to. In this case,
    the hostname where the VIP is active.
  - ``service`` the OpenStack service API is one of:
    - ``ceilometer-api``, for the API endpoint check ``/v2/capabilities``
    - ``cinder-api``, for the API endpoint check ``/``
    - ``cinder-v2-api``, for the API endpoint check  ``/``
    - ``glance-api``, for the API endpoint check  ``/``
    - ``heat-api``, for the API endpoint check  ``/``
    - ``heat-cfn-api``, for the API endpoint check  ``/``
    - ``keystone-public-api``, for the API endpoint check  ``/``
    - ``neutron-api``, for the API endpoint check  ``/``
    - ``nova-api``, for the API endpoint check ``/``
    - ``swift-api``, for the API endpoint check ``/healthcheck``
    - ``swift-s3-api``, for the API endpoint check ``/healthcheck``

|

* ``openstack_check_local_api``, the OpenStack service API status
  checked locally to the node where the service is running.
  The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.

  .. note:: All checks except for Ceilometer are performed without authentication.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to. In this case,
    the hostname where the VIP is active.
  - ``service`` the OpenStack service API is one of:
    - ``ceilometer-api``, for the API endpoint check ``/v2/capabilities``
    - ``cinder-api``, for the API endpoint check ``/``
    - ``cinder-v2-api``, for the API endpoint check  ``/``
    - ``glance-api``, for the API endpoint check  ``/``
    - ``heat-api``, for the API endpoint check  ``/``
    - ``heat-cfn-api``, for the API endpoint check  ``/``
    - ``keystone-public-api``, for the API endpoint check  ``/``
    - ``neutron-api``, for the API endpoint check  ``/``
    - ``nova-api``, for the API endpoint check ``/``
    - ``swift-api``, for the API endpoint check ``/healthcheck``
    - ``swift-s3-api``, for the API endpoint check ``/healthcheck``

API response time metrics
^^^^^^^^^^^^^^^^^^^^^^^^^

* ``openstack_<service>_http_response_times``, the HTTP response time statistics.
  The values returned are ``min``, ``max``, ``sum``, ``count``, ``upper_90``
  (90 percentile) over 10 second intervals where ``<service>`` is one of ``cinder``,
  ``glance``, ``heat`` ``keystone``, ``neutron``, ``nova`` ``ceilometer``.

  Dimensions:
 
  - ``hostname``, the hostname the metric applies to.
  - ``http_method``, the HTTP method used such as ``GET`` and ``POST``.
  - ``http_status``, the HTTP request status is one of ``2xx``, ``3xx``, ``4xx``, ``5xx``.

Compute metrics
^^^^^^^^^^^^^^^
.. _openstack_compute_metrics:

The following metrics are emitted for the compute nodes:

* ``openstack_nova_free_disk``, the disk space in GB available for new instances.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_free_ram``, the memory in MB available for new instances.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_free_vcpus``, the number of virtual CPU available for new
  instances.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_instance_creation_time``, the time in seconds it took to
  create a new instance.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_running_instances``, the number of running instances.

  Dimensions:

   - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_running_tasks``, the number of tasks currently executed.

  Dimensions:

   - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_used_disk``, the disk space in GB used by the instances.

  Dimensions:

   - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_used_ram``, the memory in MB used by the instances.

  Dimensions:

   - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_used_vcpus``, the number of virtual CPU used by the
  instances.

  Dimensions:

   - ``hostname``, the hostname the metric applies to.

|

* ``openstack_nova_service``, the Nova service (or worker) state.
  The value of the metric  is one of ``0`` for ``up``,
  ``1`` for ``down`` or ``2`` for ``disabled``.
 
  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the service is one of ``compute``,
    ``conductor``, ``scheduler``, ``cert`` or ``consoleauth``.
  - ``state``, the state of the service is one of ``up``,
    ``down`` or ``disabled``.

Aggregate metrics
^^^^^^^^^^^^^^^^^

The following metrics are emitted for Nova aggregates.

* ``openstack_nova_aggregate_free_disk``, the total amount of disk space in GB
  available for new instances in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

|

* ``openstack_nova_aggregate_free_ram``, the total amount of memory in MB
  available for new instances in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

|

* ``openstack_nova_aggregate_free_vcpus``, the total number of virtual CPU
  available for new instances in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

|

* ``openstack_nova_aggregate_running_instances``, the total number of running
  instances in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

|

* ``openstack_nova_aggregate_running_tasks``, the total number of tasks currently
  executed in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

|

* ``openstack_nova_aggregate_used_disk``, the total amount of disk space in GB
  used by the instances in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

|

* ``openstack_nova_aggregate_used_ram``, the total amount of memory in MB
  used by the instances in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

|

* ``openstack_nova_aggregate_used_vcpus``, the total number of virtual CPU
  used by the instances in the aggregate.

  Dimensions:

  - ``aggregate``, the aggregate name.
  - ``aggregate_id``, the aggregate Id.

Compute statistics metrics
^^^^^^^^^^^^^^^^^^^^^^^^^^

The following metrics contain statistics and aggregated values for Nova.

* ``openstack_nova_total_free_disk``, the total amount of disk space in GB
  available for new instances.

|

* ``openstack_nova_total_free_ram``, the total amount of memory in MB available
  for new instances.

|

* ``openstack_nova_total_free_vcpus``, the total number of virtual CPU
  available for new instances.

|

* ``openstack_nova_total_running_instances``, the total number of running
  instances.

|

* ``openstack_nova_total_running_tasks``, the total number of tasks currently
  executed.

|

* ``openstack_nova_total_used_disk``, the total amount of disk space in GB
  used by the instances.

|

* ``openstack_nova_total_used_ram``, the total amount of memory in MB used by
  the instances.

|

* ``openstack_nova_total_used_vcpus``, the total number of virtual CPU used by
  the instances.

|

* ``openstack_nova_instances``, the total number of instances by state.
    
  Dimensions:

  - ``state``, the state of the instance is one of ``active``,
    ``deleted``, ``error``, ``paused``, ``resumed``, ``rescued``,
    ``resized``, ``shelved_offloaded`` or ``suspended``.

|

* ``openstack_nova_services``, the total number of Nova services (or worker)
  by state.
  
  Dimensions:

  - ``service``, the name of the service is one of ``compute``,
    ``conductor``, ``scheduler``, ``cert`` or ``consoleauth``.
  - ``state``, the state of the service is one of ``up``,
    ``down`` or ``disabled``.

|

* ``openstack_nova_services_percent``, the percentage of Nova
  services (or workers) by state.
  
  Dimensions:

  - ``service``, the name of the service is one of ``compute``,
    ``conductor``, ``scheduler``, ``cert`` or ``consoleauth``.
  - ``state``, the state of the service is one of ``up``,
    ``down`` or ``disabled``.

Identity metrics
^^^^^^^^^^^^^^^^
.. _openstack_identity_metrics:

The following metrics are obtained from Keystone.

* ``openstack_keystone_roles``, the total number of roles.

|

* ``openstack_keystone_tenants``, the number of tenants by state.

  Dimensions:

  - ``state``, the state of the tenants is one of
    ``enabled`` or ``disabled``.

|

* ``openstack_keystone_users``, the number of users by state. 

  Dimensions:

  - ``state``, the state of the users is one of
    ``enabled`` or ``disabled``.

Volume metrics
^^^^^^^^^^^^^^
.. _openstack_volume_metrics:

The following metrics are emitted per volume node:

* ``openstack_cinder_service``, the Cinder service (or worker) state.
  The value of the metric is one of ``0`` for ``up``, ``1`` for ``down``
  or ``2`` for ``disabled``.
 
  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the service is one of ``volume``,
    ``backup``, or ``scheduler``.
  - ``state``, the state of the service is one of ``up``,
    ``down`` or ``disabled``.

|

* ``openstack_cinder_volume_attachement_time``, the time in seconds it took to
  attach a volume to an instance.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``openstack_cinder_volume_creation_time``, the time in seconds it took to
  create a new volume.

  .. note:: When using Ceph as the backend storage for volumes, the ``hostname``
   value is always set to ``rbd``.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

Volume statistics metrics
^^^^^^^^^^^^^^^^^^^^^^^^^

The following metrics are retrieved from the Cinder API:

* ``openstack_cinder_snapshots``, the total number of snapshots by state.

  Dimensions:

  - ``state``, the state of the snapshot is one of ``available``, ``creating``,
    ``attaching``, ``in-use``, ``deleting``, ``backing-up``, ``restoring-backup``,
    ``error``, ``error_deleting``, ``error_restoring``, ``error_extending``.

|

* ``openstack_cinder_snapshots_size``, the total size (in bytes) of snapshots
  by state.

  Dimensions:

  - ``state``, the state of the snapshot is one of ``available``, ``creating``,
    ``attaching``, ``in-use``, ``deleting``, ``backing-up``, ``restoring-backup``,
    ``error``, ``error_deleting``, ``error_restoring``, ``error_extending``.

|

* ``openstack_cinder_volumes``, the number of volumes by state.

  Dimensions:

  - ``state``, the state of the snapshot is one of ``available``, ``creating``,
    ``attaching``, ``in-use``, ``deleting``, ``backing-up``, ``restoring-backup``,
    ``error``, ``error_deleting``, ``error_restoring``, ``error_extending``.

|

* ``openstack_cinder_volumes_size``, the total size (in bytes) of volumes by
  state.
  
  Dimensions:

  - ``state``, the state of the snapshot is one of ``available``, ``creating``,
    ``attaching``, ``in-use``, ``deleting``, ``backing-up``, ``restoring-backup``,
    ``error``, ``error_deleting``, ``error_restoring``, ``error_extending``.

|

* ``openstack_cinder_services``, the total number of Cinder services (or worker)
  by state.

  Dimensions:

  - ``service``, the name of the service is one of ```volume``,
    ``backup``, or ``scheduler``.
  - ``state``, the state of the service is one of ``up``,
    ``down`` or ``disabled``.

|

* ``openstack_cinder_services_percent``, the percentage of Cinder
  services by state.

  Dimensions:

  - ``service``, the name of the service is one of ```volume``,
    ``backup``, or ``scheduler``.
  - ``state``, the state of the service is one of ``up``,
    ``down`` or ``disabled``.

Image metrics
^^^^^^^^^^^^^
.. _openstack_image_metrics:

The following metrics are obtained from Glance:

* ``openstack_glance_images``, the number of images by state and visibility.

  Dimensions:

  - ``state``, the state of the image is one of ``queued``,
    ``saving``, ``active``, ``killed``, ``deleted``, ``pending_delete``.
  - ``visibility``, the visibility of the image is one of
    ``public``, ``private``, ``shared``, ``community``.

|

* ``openstack_glance_images_size``, the total size (in bytes) of images by
  state and visibility.

  Dimensions:

  - ``state``, the state of the image is one of ``queued``,
    ``saving``, ``active``, ``killed``, ``deleted``, ``pending_delete``.
  - ``visibility``, the visibility of the image is one of
    ``public``, ``private``, ``shared``, ``community``.

|

* ``openstack_glance_snapshots``, the number of snapshot images by state and
  visibility.

  Dimensions:

  - ``state``, the state of the image is one of ``queued``,
    ``saving``, ``active``, ``killed``, ``deleted``, ``pending_delete``.
  - ``visibility``, the visibility of the image is one of
    ``public``, ``private``, ``shared``, ``community``.

|

* ``openstack_glance_snapshots_size``, the total size (in bytes) of snapshots
  by state and visibility.

  Dimensions:

  - ``state``, the state of the image is one of ``queued``,
    ``saving``, ``active``, ``killed``, ``deleted``, ``pending_delete``.
  - ``visibility``, the visibility of the image is one of
    ``public``, ``private``, ``shared``, ``community``.

Network metrics
^^^^^^^^^^^^^^^
.. _openstack_network_metrics:

The following metrics are obtained from Neutron:

* ``openstack_neutron_floatingips``, the total number of floating IP addresses by state.

  Dimensions:

  - ``state``, the state is one of ``active``, ``build``, ``down``, ``error``.

|

* ``openstack_neutron_networks``, the total number of virtual networks by state.
  
  Dimensions:

  - ``state``, the state is one of ``active``, ``build``, ``down``, ``error``.

|

* ``openstack_neutron_ports``, the total number of virtual ports by owner and state.

  Dimensions:

  - ``state``, the state is one of ``active``, ``build``, ``down``, ``error``.
  - ``owner``, the owner is one of ``compute``, ``dhcp``, ``floatingip``,
    ``floatingip_agent_gateway``, ``router_interface``, ``router_gateway``,
    ``router_ha_interface``, ``router_interface_distributed``,
    ``router_centralized_snat``.

|

* ``openstack_neutron_routers``, the total number of virtual routers by state.

  Dimensions:

  - ``state``, the state is one of ``active``, ``build``, ``down``, ``error``.

|

* ``openstack_neutron_subnets``, the total number of virtual subnets.

Network agent metrics
^^^^^^^^^^^^^^^^^^^^^

.. note:: These metrics are not collected when Contrail is installed.

* ``openstack_neutron_agent``, the state of the Neutron agent by service.
  The value of the metric is ``0`` for ``down, ``1`` for ``up``, ``2`` for ``disabled``.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the service that is one of ``dhcp``, ``l3``,
    ``metadata``, ``openvswitch``.

|

* ``openstack_neutron_agents``, the total number of Neutron agents by service
  and state.
  
  Dimensions:

  - ``service``, the name of the service that is one of ``dhcp``, ``l3``,
    ``metadata``, ``openvswitch``.
  - ``state``, the state of the agents is one of ``up``, ``down`` or ``disabled``.

|

* ``openstack_neutron_agents_percent``, the percentage of Neutron
  agents by state.
  
  Dimensions:

  - ``service``, the name of the service that is one of ``dhcp``, ``l3``,
    ``metadata``, ``openvswitch``.
  - ``state``, the state of the agents is one of ``up``, ``down`` or ``disabled``.

Log metrics
^^^^^^^^^^^

* ``log_messages``, the number of log messages per second by service and state.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service`` the name of the OpenStack service like ``cinder``, ``nova``, ``neutron``
    the metric applies to.
  - level, the syslog severity level is one of ``debug``, ``info``, ``warning``, and so forth.