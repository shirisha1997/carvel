# Logstash Package 

Logstash is an open source data processing engine. It ingests data from multiple sources, processes it, and sends the output to final destination in real-time. It is a core component of the ELK stack.

### Logstash parameters

|Parameter|Description|Type|Default|
|---------|-----------|----|-------|
|pullPolicy|Logstash image pull policy|string|IfNotPresent|
|replicas|Number of Logstash replicas to deploy|integer|1|
|podManagementPolicy|Pod management policy|string|OrderedReady|
|livenessProbe.httpGet.path|Request path for livenessProbe|string|/|
|livenessProbe.httpGet.port|Port for livenessProbe|string|monitoring|
|livenessProbe.initialDelaySeconds|Initial delay seconds for livenessProbe|integer|60|
|livenessProbe.periodSeconds|Period seconds for livenessProbe|integer|10|
|livenessProbe.timeoutSeconds|Timeout seconds for livenessProbe|integer|5|
|livenessProbe.failureThreshold|Failure threshold for livenessProbe|integer|6|
|livenessProbe.successThreshold|Success threshold for livenessProbe|integer|1|
|readinessProbe.httpGet.path|Request path for readinessProbe|string|/|
|readinessProbe.httpGet.port|Port for readinessProbe|string|monitoring|
|readinessProbe.initialDelaySeconds|Initial delay seconds for readinessProbe|integer|60|
|readinessProbe.periodSeconds|Period seconds for readinessProbe|integer|10|
|readinessProbe.timeoutSeconds|Timeout seconds for readinessProbe|integer|5|
|readinessProbe.failureThreshold|Failure threshold for readinessProbe|integer|6|
|readinessProbe.successThreshold|Success threshold for readinessProbe|integer|1|
|ingress.enabled|Enable ingress controller resource|string|FALSE|
|ingress.pathType|Ingress Path type|string|ImplementationSpecific|
|ingress.apiVersion|Override API Version (automatically detected if not set)|string|""|
|ingress.hostname|Default host for the ingress resource|string|logstash.local|
|ingress.path|The Path to Logstash. You may need to set this to / in order to use this with ALB ingress controllers|string|/|
|metrics.enabled|Enable the export of Prometheus metrics|string|FALSE|
|servicemonitor.enabled|Enable the export of Prometheus servicemonitor|string|FALSE|
|metrics.livenessProbe.httpGet.path|Request path for livenessProbe|string|/metrics|
|metrics.livenessProbe.httpGet.port|Port for livenessProbe|string|metrics|
|metrics.livenessProbe.initialDelaySeconds|Initial delay seconds for livenessProbe|integer|60|
|||||
|||||
|||||
|||||
|||||
|||||
