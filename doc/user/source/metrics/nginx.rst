Nginx metrics
^^^^^^^^^^^^^
.. _nginx_metrics:

A collection of Nginx metrics.

* ``nginx_connections_accepted``, the total number of accepted client connections.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``nginx_connections_active``, the current number of active client connections
  including Waiting connections.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``nginx_connections_handled``, the total number of handled connections.
  Generally, the value is the same as the ``nginx_connections_accepted`` metric
  value unless some resource limits have been reached.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``nginx_connections_reading``, the current number of connections where nginx
  is reading the request header.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``nginx_connections_waiting``, the current number of idle client connections
  waiting for a request.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``nginx_connections_writing``, the current number of connections where nginx
  is writing the response back to the client.
  
  dimensions:

  - hostname, the hostname the metric applies to.

* ``nginx_requests``, the total number of client requests.
  
  dimensions:

  - hostname, the hostname the metric applies to.

Nginx checks
^^^^^^^^^^^^
.. _nginx_checks:

* ``nginx_check``, check the availability status of the ``nginx`` service or process
  on a node. The value of the metric is ``1`` if the check is successful or ``0`` if the
  check is not successful.

  dimensions:

  - hostname, the hostname the metric applies to.