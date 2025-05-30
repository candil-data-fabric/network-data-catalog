# Instructions

>> **NOTE:** Make sure jitpack repository is registed in your ~/.m2/settings.xml file. Otherwise, Maven will not be able to find the candil-data-fabric dependencies

Run the Apache Camel application with JBang by executing the following command:

```bash
jbang camel@apache/camel run route.yaml --camel-version=4.10.0 --dep=mvn:com.cefriel:camel-chimera-graph:4.3.0,mvn:com.cefriel:camel-chimera-mapping-template:4.3.0,mvn:com.github.candil-data-fabric:gnmi-java:1.0.0
```
