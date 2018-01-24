# collection of frequently needed commands
## certificates
**get certifiacates and store in keystore**
```
# view certificates
openssl s_client -showcerts -connect my.host.com:443
# store desired ones to a file (myfile.pem)

# then base64 decode it
base64 -d myfile.pem > myfile.cer

# and add to keystore
keytool -import -alias gateway-identity -keystore mykeystore.jks -file myfile.cer
```

## java
- checking classpath
```bash
jar tf foo.jar | grep MyClass
```
- reload the service / restart it in case you modify the same class (just to be sure)

## big data
starting out it might be a good idea to quickly get something up and running
- cloudbreak is great
- in case you want to go for something smaller 
  - https://github.com/rmaruthiyodan/docker-hdp-lab
## spark
- assuming your cluster does not install all client code on each data node remember to ship hive-site.xml as well as the tez xml file when submitting a spark job in yarn cluster mode
- it might have worked just fine in yarn client - but will no longer work in yarn cluster without these files.
- dependency clashes: shading, but with some tricks. http://asyncified.io/2016/04/07/spark-uber-jars-and-shading-with-sbt-assembly/
- sql optimization: https://blog.deepsense.ai/optimize-spark-with-distribute-by-and-cluster-by/

**data sources**
- REST API as enrichment https://github.com/sourav-mazumder/Data-Science-Extensions/tree/master/spark-datasource-rest
**tuning**
- http://rea.tech/how-we-optimize-apache-spark-apps/
- http://fdahms.com/2015/10/04/writing-efficient-spark-jobs/


**aggregations**
- multiple aggregations
  - UADF
  - rdd statCounter
  - scalding: https://github.com/twitter/scalding/wiki/Aggregation-using-Algebird-Aggregators#composing-aggregators
  
**partition handling**
- https://towardsdatascience.com/writing-into-dynamic-partitions-using-spark-2e2b818a007a

**spark on yarn**
- vcores not chosen correctly https://stackoverflow.com/questions/25563736/yarn-is-not-honouring-yarn-nodemanager-resource-cpu-vcores/25570709#25570709

## hive 
- jdbc for other tools https://github.com/timveil/hive-jdbc-uber-jar

## hdfs shell

- counting of files in directory `hdfs dfs -count -v -h /path/to/data/*`

## python
- date handling https://www.youtube.com/watch?v=Q97vDzaNQyU


## yarn
- overview https://de.hortonworks.com/blog/yarn-capacity-scheduler/

## machine learning
### categorical handling
- http://www.win-vector.com/blog/2016/11/you-should-re-encode-high-cardinality-categorical-variables/

### cross validation
- https://www.google.at/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0ahUKEwjTtunBu53YAhXGZFAKHTkcAhoQFggqMAA&url=https%3A%2F%2Fgithub.com%2Fyandexdataschool%2Fml-training-website%2Fraw%2Fgh-pages%2Fpresentations%2FSavenkov_KaggleMercedes_2017_eng.pdf&usg=AOvVaw3Zle9OmWU-FhS9QSB_dUVK

## conversions of data

### geospatial data
- https://github.com/dice-cyfronet/ascii-grid-source/blob/master/src/main/java/pl/cyfronet/urbanflood/ogc/geoserver/data/ASCIIGridDataReader.java
- https://stackoverflow.com/a/33473452/5200303
- https://en.wikipedia.org/wiki/Ramer–Douglas–Peucker_algorithm

## ambari
- changing the password follow https://community.hortonworks.com/questions/449/how-to-reset-ambari-admin-password.html
```
1. Log on to ambari server host shell
2. Run 'psql -U ambari-server ambari'
3. Enter password 'bigdata'
4. In psql:
update ambari.users set user_password='538916f8943ec225d97a9a86a2c6ec0818c1cd400e09e03b660fdaaec4af29ddbb6f2b1033b81b00' where user_name='admin'

5. Quit psql
6. Run 'ambari-server restart'

This will reset the admin account back to the password of 'admin'
```
