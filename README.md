alfresco-purge
==============

After some time, deleting contents can fill the Alfresco's trashcan and removing nodes manually with the UI can be unpractical (users always forget about this). Alfresco does not actually delete content, but moves deleted nodes into the archive store, which is like a trashcan. Deleted contents can stay there forever, until users decide to clean-up the trashcan. In a big repository this could lead to a huge waste of resources.  I need a service I can invoke programmatically to empty the trashcan, for example by scheduling a task with an external job.