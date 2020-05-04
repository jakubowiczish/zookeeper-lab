# Run

For task 4 (run these commands in ```bin``` directory, all in separate terminals):

Server 1:

```bash
.\zkServer2.cmd \zoo1.cfg
```

Client 1:

```bash
.\zkCli.cmd -server 127.0.0.1:2181
```

Server 2:

```bash
.\zkServer2.cmd \zoo2.cfg
```

Client 2:

```bash
.\zkCli.cmd -server 127.0.0.1:2182
```

Server 3:

```bash
.\zkServer2.cmd \zoo3.cfg
```

Client 3:

```bash
.\zkCli.cmd -server 127.0.0.1:2183
```

Already configured well in ```conf```

In the main directory of your disk, there should be ```Zookeeper``` directory with its content,
for instance: 

```
D:\Zookeeper
```

#

# Apache ZooKeeper
![alt text](https://zookeeper.apache.org/images/zookeeper_small.gif "ZooKeeper")

For the latest information about Apache ZooKeeper, please visit our website at:

   http://zookeeper.apache.org/

and our wiki, at:

   https://cwiki.apache.org/confluence/display/ZOOKEEPER

## Packaging/release artifacts

Either downloaded from https://zookeeper.apache.org/releases.html or
found in zookeeper-assembly/target directory after building the project with maven.

    apache-zookeeper-[version].tar.gz

        Contains all the source files which can be built by running:
        mvn clean install

        To generate an aggregated apidocs for zookeeper-server and zookeeper-jute:
        mvn javadoc:aggregate
        (generated files will be at target/site/apidocs)

    apache-zookeeper-[version]-bin.tar.gz

        Contains all the jar files required to run ZooKeeper
        Full documentation can also be found in the docs folder

As of version 3.5.5, the parent, zookeeper and zookeeper-jute artifacts
are deployed to the central repository after the release
is voted on and approved by the Apache ZooKeeper PMC:

  https://repo1.maven.org/maven2/org/apache/zookeeper/zookeeper/

## Java 8

If you are going to compile with Java 1.8, you should use a
recent release at u211 or above. 

## Contributing
We always welcome new contributors to the project! See [How to Contribute](https://cwiki.apache.org/confluence/display/ZOOKEEPER/HowToContribute) for details on how to submit patch through pull request and our contribution workflow.


