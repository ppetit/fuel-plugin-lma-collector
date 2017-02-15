LMA metrics
-----------
.. _lma_metrics:

A collection of StackLight related (self-monitoring) metrics. 

LMA system metrics
^^^^^^^^^^^^^^^^^^

These metrics have a ``service`` dimension which contains the name of the
process or service it applies to.
The values can be: ``hekad``, ``collectd``, ``influxd``, ``grafana-server``
or ``elasticsearch``.

* ``lma_components_processes``, the number of processes currently running.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.

|

* ``lma_components_threads``, the number of threads currently running.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.

|

* ``lma_components_cputime_syst``, the percentage of CPU time spent in system
  mode by the service. It can be greater than 100% when the node has more than
  one CPU.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.

|

* ``lma_components_cputime_user``, the percentage of CPU time spent in user
  mode by the service. It can be greater than 100% when the node has more than
  one CPU.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.

|

* ``lma_components_disk_bytes_read``, the number of bytes read from disk(s) per
  second.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_disk_bytes_write``, the number of bytes written to disk(s)
  per second.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_disk_ops_read``, the number of read operations from disk(s)
  per second.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_disk_ops_write``, the number of write operations to disk(s)
  per second.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_memory_code``, the physical memory devoted to executable code
  in bytes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_memory_data``, the physical memory devoted to other than
  executable code in bytes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_memory_rss``, the non-swapped physical memory used in bytes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_memory_virtual``, the virtual memory size in bytes.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_pagefaults_majflt``, major page faults per second.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_pagefaults_minflt``, minor page faults per second.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.
  
|

* ``lma_components_stacksize``, the absolute value of the start address (the bottom)
  of the stack minus the address of the current stack pointer.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - ``service``, the name of the process or service.

Heka pipeline metrics
^^^^^^^^^^^^^^^^^^^^^

Note that by default, the Heka pipeline metrics are
disabled to reduce the workload on the ``hekad`` process.

The metrics for both types are as follows:

* ``hekad_memory``, the total memory in bytes used by the Sandbox.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - name, the name of the Heka plugin.
  - type, the type of Heka plugin that can be either ``decoder`` or ``filter``.

|

* ``hekad_msg_avg_duration``, the average time in nanoseconds for processing
  the message.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - name, the name of the Heka plugin.
  - type, the type of Heka plugin that can be either ``decoder`` or ``filter``.

|

* ``hekad_msg_count``, the total number of messages processed by the decoder.
  This resets to ``0`` when the process is restarted.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - name, the name of the Heka plugin.
  - type, the type of Heka plugin that can be either ``decoder`` or ``filter``.

|

Additional metrics for the ``filter`` type only:

|

* ``hekad_timer_event_avg_duration``, the average time in nanoseconds for
  executing the ``timer_event`` function.

  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - name, the name of the Heka plugin.
  - type, the type of Heka plugin ``filter``.

|

* ``hekad_timer_event_count``, the total number of the
  ``timer_event`` function calls. This resets to ``0`` when
  ``hekad`` is restarted.
  
  Dimensions:

  - ``hostname``, the hostname the metric applies to.
  - name, the name of the Heka plugin.
  - type, the type of Heka plugin ``filter``.