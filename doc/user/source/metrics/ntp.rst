NTP metrics
^^^^^^^^^^^
.. _ntp_metrics:

A collection of NTP related metrics.

* ``ntp_frequency_offset_loop``, the 'pll frequency' value returned by 'ntpdc -c kerninfo'

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``ntp_time_dispersion_peer``, the maximum errors of the local clock relative to the reference
  'peer' NTP server clock. 

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``server``, the ``peer`` NTP server.

|

* ``ntp_time_offset_error``, the 'estimated error' value returned by 'ntpdc -c kerninfo'

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``ntp_time_offset_loop``, the 'pll offset' value returned by ntpdc -c kerninfo

  Dimensions:

  - ``hostname``, the hostname the metric applies to.

|

* ``ntp_time_offset_peer``, the time difference to adjust the local clock to bring it in
  sync with the 'peer' NTP server clock in microseconds.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``server``, the 'peer' NTP server.