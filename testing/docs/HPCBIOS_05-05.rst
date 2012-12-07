.. _HPCBIOS_05-05:

HPCBIOS_05-05: Common Queue Names
=================================

.. note::
  Common queue names will allow users to understand HPCBIOS HPC
  environment faster and move scripts across sites more easily.

  * BC Policy: HPCBIOS_05-05
  * Date of Policy: 2012-12-15

A goal of this policy is to institute a core namespace of batch queues
with the same names at each of the centers participating in the Baseline
Configuration Initiative. The queue names were chosen to align with HPCBIOS
project priorities. In addition, each center is explicitly allowed to
offer customized batch support and service levels for specialized work
loads of each own.

The core set of common queue names will allow users to more easily move
their jobs and scripts among centers. This improves user productivity by
requiring less time and effort to support many different scripts and to
learn a different queue environment at each center.

The Compute queue names defined by this project and their respective
priority classes are:

+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| Queue Name    | Priority Class   | Cost factor   | Policy SLA   | Description                                | Specifications                                          |
+===============+==================+===============+==============+============================================+=========================================================+
| urgent        | Urgent           | 1             | MAY          | Approved by Site                           | as needed, for fulfilling site or project objectives.   |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| interactive   | Interactive      | 1             | MAY          | For interactive jobs                       | maxsize @ 4 nodes; max walltime @ 2 hours               |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| debug         | Debug            | 0             | SHOULD       | Time/Resource limited for debug purposes   | max walltime @ 30 minutes                               |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| batch         | Standard         | 1             | MUST         | For approved HPCBIOS projects              | maxsize @ 50% of resources ; max walltime @ 24hours     |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| transfer      | Standard         | 1             | MAY          | Data stage-in/stage-out jobs               | used for jobs heavy in I/O meant for data transfers     |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| gpu           | Standard         | 1             | MAY          | For approved HPCBIOS projects needing GPUs | Normal queue for GPU resources                          |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| gpu-low       | Low Priority     | 0             | MAY          | For approved HPCBIOS projects needing GPUs | No allocation subtraction                               |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+
| batch-low     | Low Priority     | 0             | MAY          | For approved HPCBIOS projects              | No allocation subtraction                               |
+---------------+------------------+---------------+--------------+--------------------------------------------+---------------------------------------------------------+

The above list of queues, starting at urgent and ending at batch-low,
denotes priorities from the highest to lowest, in that order.
