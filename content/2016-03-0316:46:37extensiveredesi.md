extensive redesign ob elasticsearch access abstraction: added another
=====================================================================

Date: 2016-03-03 16:46:37

``` {style="white-space:pre-wrap;width:81ex"}
extensive redesign ob elasticsearch access abstraction: added another
abstraction layer with the class ElasticseachClient. This enables us now
to access an external elasticsearch cluster as transport client. If such
an access method is choosed, the configuration parameters in
config.properties with prefix 'elasticsearch_transport' must be set
accordingly.
```
