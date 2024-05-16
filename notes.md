# Distributed Training Notes

## Deciding on a master node for cluster management

- Zookeeper
  - Znodes: Hybrid of file/directory. File that can have child nodes
    - Persistent and ephemeral
  - Leader election algorithm
    - Chooses a leader node between multiple cluster nodes
  - Go to Zookeeper directory: `cd ~/apache-zookeeper-3.8.4-bin/bin`
  - Start Zookeeper server: `./zkServer.sh start`
  - Start Zookeeper CLI: `./zkCli.sh`
    - Create znode: `create /parent "some parent data"`
    - `ls /parent`
    - View details: `get /parent`
    - Delete znode: `rmr /parent`
