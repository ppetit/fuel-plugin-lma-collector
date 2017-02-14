HAProxy  metrics
----------------

A collection of HAProxy related metrics.

.. _haproxy_metrics:


* ``haproxy_connections``, the number of current connections.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``haproxy_pipes_free``, the number of free pipes.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``haproxy_pipes_used``, the number of used pipes.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``haproxy_run_queue``, the number of connections waiting in the queue.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``haproxy_ssl_connections``, the number of current SSL connections.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``haproxy_tasks``, the number of tasks.

  dimensions:

  - hostname, the hostname the metric applies to.

* ``haproxy_uptime``, the HAProxy service uptime in seconds.

  dimensions:

  - hostname, the hostname the metric applies to.

HAProxy frontend and backend metrics
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The HAProxy frontend and backend metrics have a ``frontend`` or
``backend`` dimension that can take different values depending on the
configuration of HAProxy in your deployment.
By default, both the ``frontend`` and ``backend`` dimensions can take
the following values:

* aodh-api
* backend
* cinder_api
* contrail_api
* contrail_discovery
* glance_api
* glance_registry_api
* haproxy_backend_bytes_in
* heat_api
* heat_cfn_api
* heat_cloudwatch_api
* horizon-web (when Horizon is deployed without TLS)
* horizon-https (when Horizon is deployed with TLS)
* keystone_admin_api
* keystone_public_api
* murano-api
* mysql_cluster
* mysqld-tcp
* neutron_api
* nova_api
* nova-metadata-api
* nova-novncproxy-websocket
* nova_metadata_api
* rabbitmq_cluster
* sahara-api
* swift-api

Frontend metrics
^^^^^^^^^^^^^^^^
.. _haproxy_frontend_metric:

* ``haproxy_frontend_bytes_in``, the number of bytes received by the frontend.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.
  
* ``haproxy_frontend_bytes_out``, the number of bytes transmitted by the frontend.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_denied_requests``, the number of denied requests.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_denied_responses``, the number of denied responses.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_error_requests``, the number of error requests.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_response_1xx``, the number of HTTP responses with 1xx code.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_response_2xx``, the number of HTTP responses with 2xx code.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_response_3xx``, the number of HTTP responses with 3xx code.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_response_4xx``, the number of HTTP responses with 4xx code.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_response_5xx``, the number of HTTP responses with 5xx code.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_response_other``, the number of HTTP responses with other code.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_session_current``, the number of current sessions.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_frontend_session_total``, the cumulative number of sessions.

  dimensions:

  - frontend, the name of the frontend service endpoint.
  - hostname, the hostname the metric applies to.


Backend metrics
^^^^^^^^^^^^^^^
.. _haproxy_backend_metric:

* ``haproxy_backend_bytes_in``, the number of bytes received by the backend
  service endpoint.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_bytes_out``, the number of bytes transmitted by the
  backend service endpoint.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_denied_requests``, the number of denied requests.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_denied_responses``, the number of denied responses.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_downtime``, the total downtime in seconds.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_error_connection``, the number of error connections.
  
  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_error_responses``, the number of error responses.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_queue_current``, the number of requests in queue.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_redistributed``, the number of times a request was
  dispatched to another service endpoint.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_response_1xx``, the number of HTTP responses with 1xx code.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_response_2xx``, the number of HTTP responses with 2xx code.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_response_3xx``, the number of HTTP responses with 3xx code.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_response_4xx``, the number of HTTP responses with 4xx code.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_response_5xx``, the number of HTTP responses with 5xx code.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_response_other``, the number of HTTP responses with other
  code.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_retries``, the number of times a connection to a server
  was retried.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_server``, the state of the backend service endpoint
  in the HAProxy cluster where a value:

  - ``0`` represents ``down``.
  - ``1`` represents ``up``.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.
  - state, the state of the backend service endpoint
  - server, the hostname where the backend service endpoint is running.

  Note that this metric (and the following) has two additional dimensions.
  
  A ``state`` dimension that contains the state of the backend service
    endpoint where:

    - ``0`` represents ``down``.
    - ``1`` represent ``up``.

  A ``server`` dimension that contains the hostname the state of the backend
  service endpoint applies to.


* ``haproxy_backend_servers``, the number of backend service endpoints grouped
  by state. This metric has an additional ``state`` dimension that contains
  the state of the backend service endpoint (either 'down' or 'up').

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.
  - state, the state of the backend service endpoint (either 'down' or 'up').

* ``haproxy_backend_servers_percent``, the percentage of backend service
  endpoints grouped by state. This metric has an additional ``state``
  dimension that contains the state of the backend service endpoint
  (either 'down' or 'up').
  
  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.
  - state, the state of the backend service endpoint (either 'down' or 'up').

* ``haproxy_backend_session_current``, the number of current sessions.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_session_total``, the cumulative number of sessions.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

* ``haproxy_backend_status``, the cluster state of the backend service
  endpoint where value:
  
  - ``0`` represents ``down``
  - ``1`` represents ``up``.

  dimensions:

  - backend, the name of the backend service endpoint.
  - hostname, the hostname the metric applies to.

HAProxy checks
^^^^^^^^^^^^^^
.. _haproxy_checks:

* ``haproxy_check``, check the availability status of the HAProxy service.
  The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.

  dimensions:
  
  - hostname, the hostname the metric applies to.