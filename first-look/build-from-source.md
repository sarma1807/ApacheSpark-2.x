## Apache Spark 2.0 Build From Source Code 20-May-2016

[cass@compile spark2]$ `date` <br>
`Fri May 20 12:22:02 EDT 2016`

[cass@compile ~]$ `mkdir spark2/` <br>
[cass@compile ~]$ `cd spark2/`

[cass@compile spark2]$ `pwd` <br>
`/home/cass/spark2`

[cass@compile spark2]$ `ll` <br>
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

[cass@compile spark2]$ `cd spark/` <br>

[cass@compile spark2]$ `pwd` <br>
`/home/cass/spark2/spark`

[cass@compile spark]$ `build/mvn -DskipTests clean package` <br>
`### build log/output is published as a sperate file on this github location ###` <br>
https://github.com/sarma1807/ApacheSpark2.x/blob/master/first-look/build-from-source-BuildOutput.md

#### Build process took nearly 15 minutes.
