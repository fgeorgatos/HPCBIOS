.. _HPCBIOS_05-05:

HPCBIOS_05-05: Common Queue Names
=================================

.. note::
  Common queue names will allow users to understand HPCBIOS compatible resources faster,
  select appropriate queues and, move workflows across sites without related issues.

  * BC Policy: HPCBIOS_05-05
  * Date of Policy: 2012-12-15

The goal of this policy is to institute a core namespace of batch queues
with the same names at each of the systems participating in a Baseline Configuration.
The queue names were chosen to align with collective experience from multiple HPC sites.
In addition, each system or site is explicitly
allowed to offer customized batch support and service levels for specialized workloads
or projects of each own.
Systems MAY have more queues on as needed basis and SHOULD extend this policy in a backward-compatible way.

The core set of common queue names will allow users to more easily move
their jobs and scripts among systems. This improves user productivity by
requiring less time and effort to support many different scripts
and to learn a different queue environment at each site.

The Compute queue names defined by HPCBIOS and their respective priority classes are:

+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| Queue Name    | Priority Class   | Cost factor   | Policy SLA   | Description                                | Specifications to meet (ie. minimum maxima)             |
+===============+==================+===============+==============+============================================+=========================================================+
| urgent        | Urgent           | 1             | MAY          | Approved by Site                           | as needed, for fulfilling site or project objectives    |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| interactive   | Interactive      | 1             | MAY          | For interactive jobs                       | maxsize @ 4 nodes; max. walltime @ 2 hours              |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| debug         | Debug            | 0             | SHOULD       | Time/Resource limited for debug purposes   | max. walltime @ 30 minutes                              |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| gpu           | Standard         | 1             | MAY          | For approved projects needing GPUs         | Normal queue for GPU resources                          |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| batch         | Standard         | 1             | MUST         | For approved projects - GENERIC            | maxsize @ 50% of resources ; max. walltime @ 24hours    |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| transfer      | Standard         | 1             | MAY          | Data stage-in/stage-out jobs               | used for jobs heavy in I/O, meant for data transfers    |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| gpu-low       | Low Priority     | 0             | MAY          | For approved projects needing GPUs         | No allocation subtraction, possibly best-effort         |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| batch-low     | Low Priority     | 0             | MAY          | For approved projects                      | No allocation subtraction, possibly best-effort         |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+

The above list of queues, scaling among *urgent* and *batch-low*,
denotes different level of priorities, ranging from the highest to lowest.

A site still maintains the right to choose which users have access to which queues
and at which times, so essentially compliance with this policy is quite flexible.

Potential sources of information for further future upgrades of this policy include:
  * http://centers.hpc.mil/consolidated/bc/policies.php?choice=queue
  * http://centers.hpc.mil/consolidated/bc/policies.php?choice=common
  * http://centers.hpc.mil/consolidated/bc/commonCommands.php?choice=show_queues
  * http://www.nersc.gov/users/computational-systems/hopper/running-jobs/queues-and-policies/
  * http://trac.mcs.anl.gov/projects/cobalt/wiki/DebugQueueConfig

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS maintainers.
