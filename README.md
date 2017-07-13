Role Name
=========


Requirements
------------


Role Variables
--------------

# The prefix to be used for the daily snapshot name. The full name will be
# appended with timestamp.
daily_snapshot_name_prefix:

# The snapshot repository name to be used in the es s3 snapshot plugin and in
# the making snapshot routine. For each elasticsearch cluster it has its own
# unique name (thus we can use one s3 bucket to store multiple elasticsearch
# cluster snapshot).
snapshot_repository_name:

# The full endpoint url of the elasticsearch cluster. Used to talk to es in
# registering the snapshot repository name and post es command for maintenance.
es_cluster_endpoint:

# How many months we keep the es indices in the system? The index of the older
# month will be deleted.
es_months_to_keep_indices:

# The s3 bucket name to be used as es snapshot storage.
es_snapshot_bucket_name:

Dependencies
------------


Example Playbook
----------------


License
-------

BSD

Author Information
------------------

