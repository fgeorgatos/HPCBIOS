.. _HPCBIOS_2012-98:

HPCBIOS_2012-98: Common Set of Environment Variables
====================================================

.. note::

  This policy is written to define a core set of environment variables that represent
  the a resource definition at each of the HPCBIOS designated centers participating
  in the Baseline Configuration (BC) Initiative. These variables shall be pre-defined
  in all login scripts, making them automatically available to users at each center,
  whenever the relevant functionality is in place.

  * BC Policy: HPCBIOS_2012-98
  * Date of Policy: 2012-12-15

The current list of variables has as follows:

BC_CORES_PER_NODE (MUST)
  This variable contains the number of cores per node for the compute node type to which a job is being submitted.

BC_MEM_PER_NODE (MUST)
  This variable contains the approximate maximum memory per node available to an end user program (in integer MBs) for the compute node type to which a job is being submitted.

BC_MPI_TASKS_ALLOC (SHOULD)
  This variable, intended to be referenced from inside a job script, shall contain the number of MPI tasks that are allocated for a particular job.

BC_NODE_ALLOC (SHOULD)
  This variable, intended to be referenced from inside a job script, shall contain the number of nodes allocated for a particular job.

JAVA_HOME (SHOULD)
  This variable contains the path to the base directory of the default installation of JAVA on a particular compute platform. If the platform does not have JAVA installed, this variable should not be defined. It can also be provided via the modules mechanism.

SAMPLES_HOME (MUST)
  This variable contains the path to the base directory for the sample codes and scripts installed by a center's staff under BC policy Sample Code Repository.

SOFT_HOME (MUST)
  This variable contains the path to the base directory for the application codes installed on a system.

WORK (MUST) 
  Same as WORKDIR, see below

WORKDIR (SHOULD)
  This is an individual user’s directory on the local temporary file system (i.e., local high speed disk) that is available on all HPCBIOS high performance computing (HPC) systems. WORK is intended to be used by executing programs to perform file I/O that is local to that system in order to avoid slower file I/O across a network mounted file system, such as a user's HOME or ARCHIVE directories. It is not intended to be used as a permanent file storage area by users, rather as working area between tasks. Accordingly, this file system MAY NOT be backed up or exported to any other system. In the event of file or directory structure deletion or a catastrophic disk failure, such files and directory structures are lost. Thus, it is the user’s responsibility to transfer files that need to be saved to a location that allows for permanent file storage, such as the user’s archival or home directory locations - if they are permanent via a backup policy or, another external system.

This list of environment variables is subject to change, and should be reviewed on a periodic basis for potential additions, modifications or deletions.

