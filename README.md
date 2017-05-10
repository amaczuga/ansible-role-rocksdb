Role Name
=========

Install RocksDB software (http://rocksdb.org/)

Requirements
------------

None

Role Variables
--------------

```yaml
# software install destination directory
rocksdb_install_dir: "/usr/local"

rocksdb_sw_name: "rocksdb"

# software version
rocksdb_sw_release: "5.2.1"

# software source archive location
rocksdb_sw_release_archive: "https://github.com/facebook/rocksdb/archive/v{{ rocksdb_sw_release }}.tar.gz"
```

Dependencies
------------

none

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: amaczuga.rocksdb, rocksdb_install_dir: "/opt" }

License
-------

Apache 2.0

Author Information
------------------

andrzej maczuga
