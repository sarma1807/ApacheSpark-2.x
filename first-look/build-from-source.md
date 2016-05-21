## Apache Spark 2.0 Build From Source Code 20-May-2016

[cass@compile spark2]$ `date`
`Fri May 20 12:22:02 EDT 2016`

[cass@compile ~]$ `mkdir spark2/`
[cass@compile ~]$ `cd spark2/`

[cass@compile spark2]$ `pwd`
`/home/cass/spark2`

[cass@compile spark2]$ `ll`
`total 0`

[cass@compile spark2]$ `git clone https://github.com/apache/spark.git`
```
Cloning into 'spark'...
remote: Counting objects: 358916, done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 358916 (delta 4), reused 0 (delta 0), pack-reused 358901
Receiving objects: 100% (358916/358916), 176.55 MiB | 3.35 MiB/s, done.
Resolving deltas: 100% (136733/136733), done.
```

[cass@compile spark2]$ `cd spark/`

[cass@compile spark2]$ `pwd`
`/home/cass/spark2/spark`

[cass@compile spark]$ `build/mvn -DskipTests clean package`
`### build log/output is published as a sperate file on this github location ###`

#### Build process took nearly 15 minutes.
