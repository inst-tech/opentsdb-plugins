Executable jar so you can test plugins. 


Create a "lib" folder and put the OpenTSDB jar there.


```
gradle clean; gradle fatJar; java -jar build/libs/DiscoveryPlugins-all-1.0-SNAPSHOT.jar --config src/main/resources/opentsdb.conf
```

```
19:58:20.113 [main] INFO  i.t.o.discoveryplugins.ExecutePlugin - Starting.
19:58:20.120 [main] INFO  net.opentsdb.utils.Config - Successfully loaded configuration file: src/main/resources/opentsdb.conf
19:58:20.122 [main] DEBUG i.t.o.discoveryplugins.CuratorPlugin - constructor called
19:58:20.123 [main] INFO  i.t.o.discoveryplugins.CuratorPlugin - Apache Curator ServiceDiscovery Plugin Initialized
19:58:20.123 [main] DEBUG i.t.o.discoveryplugins.CuratorPlugin - Finished with config
19:58:20.123 [main] INFO  i.t.o.discoveryplugins.ExecutePlugin - Successfully initialized startup plugin [io.tsdb.opentsdb.discoveryplugins.CuratorPlugin] version: 2.0.0
19:58:20.123 [main] INFO  i.t.o.discoveryplugins.ExecutePlugin - 2.0.0
19:58:20.123 [main] INFO  i.t.o.discoveryplugins.ExecutePlugin - shutting down
19:58:20.123 [main] DEBUG i.t.o.discoveryplugins.CuratorPlugin - shutting down.
```