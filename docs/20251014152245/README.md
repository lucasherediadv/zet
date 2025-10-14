# Don't use mount merely to list mounted filesystems for human reading

Use `findmnt`

* Shows mountpoints in a hierarchy
* Filter mounts by type
* Use `--real` to get only "real" filesystems
* JSON output mode
