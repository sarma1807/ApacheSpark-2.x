## Apache Spark-Shell 2.0 First Look

[cass@compile spark]$ `./bin/spark-shell`
```
Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
Setting default log level to "WARN".
To adjust logging level use sc.setLogLevel(newLevel).
16/05/20 12:45:36 WARN NativeCodeLoader: Unable to load native-hadoop library for your platform... using builtin-java classes where applicable
16/05/20 12:45:36 WARN AbstractHandler: No Server set for org.spark_project.jetty.server.handler.ErrorHandler@ae73c80
Spark context Web UI available at http://192.168.0.98:4040
Spark context available as 'sc' (master = local[*], app id = local-1463762736854).
Spark session available as 'spark'.
Welcome to
      ____              __
     / __/__  ___ _____/ /__
    _\ \/ _ \/ _ `/ __/  '_/
   /___/ .__/\_,_/_/ /_/\_\   version 2.0.0-SNAPSHOT
      /_/

Using Scala version 2.11.8 (Java HotSpot(TM) 64-Bit Server VM, Java 1.8.0_92)
Type in expressions to have them evaluated.
Type :help for more information.

scala> spark
res0: org.apache.spark.sql.SparkSession = org.apache.spark.sql.SparkSession@2407a36c

scala> spark.
baseRelationToDataFrame   createDataFrame   experimental      newSession   sparkContext   streams
catalog                   createDataset     implicits         range        sql            table
conf                      emptyDataFrame    listenerManager   read         stop           udf

scala> sc
res1: org.apache.spark.SparkContext = org.apache.spark.SparkContext@31006a75

scala> sc.
accumulable             cancelAllJobs          getConf                    isStopped          range               sparkUser
accumulableCollection   cancelJobGroup         getExecutorMemoryStatus    jars               register            startTime
accumulator             clearCallSite          getExecutorStorageStatus   killExecutor       requestExecutors    statusTracker
addFile                 clearJobGroup          getLocalProperty           killExecutors      runApproximateJob   stop
addJar                  defaultMinPartitions   getPersistentRDDs          listAccumulator    runJob              submitJob
addSparkListener        defaultParallelism     getPoolForName             longAccumulator    sequenceFile        textFile
appName                 deployMode             getRDDStorageInfo          makeRDD            setCallSite         uiWebUrl
applicationAttemptId    doubleAccumulator      getSchedulingMode          master             setCheckpointDir    union
applicationId           emptyRDD               hadoopConfiguration        newAPIHadoopFile   setJobDescription   version
binaryFiles             files                  hadoopFile                 newAPIHadoopRDD    setJobGroup         wholeTextFiles
binaryRecords           getAllPools            hadoopRDD                  objectFile         setLocalProperty
broadcast               getCheckpointDir       isLocal                    parallelize        setLogLevel

scala> sc.version
res2: String = 2.0.0-SNAPSHOT

scala> exit
<console>:24: error: not found: value exit
       exit
       ^

scala> quit
<console>:24: error: not found: value quit
       quit
       ^

scala> :quit

[cass@compile spark]$
```
