# Zookeeper

## It provides various features for various distrubuted Application like
- Distributed Configuration
- Self election
- Coordination
- Key value store
- It has internal Tree Structure
    - Each node is called zNode
    - zNode are persistance
    - zNode has path
    - zNode can be watched for changes

## Roles
- Every broker rregister itself by sending heartbeats
- Maintains the list of Topic along with other Topic details like Partitions, Replication factor etc
- Election of leader if one broker goes down
- Stores the Kafka Cluster-Id

## Zookeeper Quorum Sizing, No of zookeeper server 2N+1 (1,3,5,7..). Ideally 3 should be good.


## Zookeeper Performance
- Use FAST Disk e.g SSD
- No RAM Swap
- Set Snapshot and Log on seperate Disk
- High performance Network
- Setup good number of zookeeper Server
- On Cloud setup Zookeeper in same region
- Setup Zookeeper and Kafka on seperate machines




