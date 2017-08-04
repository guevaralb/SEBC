sudo -u hdfs hdfs hdfs dfs -ls /user/

Found 7 items
drwxr-xr-x   - hdfs   supergroup          0 2017-08-04 17:12 /user/haley
drwxrwxrwx   - mapred hadoop              0 2017-08-04 17:01 /user/history
drwxrwxr-t   - hive   hive                0 2017-08-04 17:02 /user/hive
drwxrwxr-x   - hue    hue                 0 2017-08-04 17:02 /user/hue
drwxrwxr-x   - oozie  oozie               0 2017-08-04 17:02 /user/oozie
drwxr-xr-x   - hdfs   supergroup          0 2017-08-04 17:12 /user/saturn
drwxr-x--x   - spark  spark               0 2017-08-04 17:01 /user/spark

curl -uadmin:admin http://localhost:7180/api/v14/hosts
{
  "items" : [ {
    "hostId" : "1c8e7b44-c781-4f89-ae5b-7733029df413",
    "ipAddress" : "172.31.17.35",
    "hostname" : "ip-172-31-17-35.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/hostRedirect/1c8e7b44-c781-4f89-ae5b-7733029df413",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 16,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 67105165312
  }, {
    "hostId" : "cb46a3c9-0948-48f8-93db-e967926db1e3",
    "ipAddress" : "172.31.21.20",
    "hostname" : "ip-172-31-21-20.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/hostRedirect/cb46a3c9-0948-48f8-93db-e967926db1e3",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 16,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 67105165312
  }, {
    "hostId" : "fc913540-0bcc-47e1-9c67-caa01642f383",
    "ipAddress" : "172.31.26.16",
    "hostname" : "ip-172-31-26-16.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/hostRedirect/fc913540-0bcc-47e1-9c67-caa01642f383",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 16,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 67105165312
  }, {
    "hostId" : "01b0f7b4-f130-4918-af5f-74fee859f6b0",
    "ipAddress" : "172.31.30.206",
    "hostname" : "ip-172-31-30-206.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/hostRedirect/01b0f7b4-f130-4918-af5f-74fee859f6b0",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 16,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 67105165312
  } ]
}

curl -uadmin:admin http://localhost:7180/api/v8/clusters/services
{
  "message" : "Cluster 'services' not found."
}

[root@ip-172-31-30-206 ~]# curl  -uadmin:admin http://localhost:7180/api/v8/clustes/guevaralb/services
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/serviceRedirect/hive",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/serviceRedirect/zookeeper",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/serviceRedirect/hue",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/serviceRedirect/oozie",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/serviceRedirect/yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)"
  }, {
    "name" : "spark_on_yarn",
    "type" : "SPARK_ON_YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/serviceRedirect/spark_on_yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Spark"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-30-206.ec2.internal:7180/cmf/serviceRedirect/hdfs",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS"
  } ]
}

