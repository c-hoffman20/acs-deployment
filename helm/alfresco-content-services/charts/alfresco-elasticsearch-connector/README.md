# alfresco-elasticsearch-connector

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 3.0.0](https://img.shields.io/badge/AppVersion-3.0.0-informational?style=flat-square)

A Helm chart for deploying Alfresco Elasticsearch connector

Please refer to the [documentation](https://github.com/Alfresco/acs-deployment/blob/master/docs/helm/README.md) for information on the Helm charts and deployment instructions.

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| file://../alfresco-content-common | alfresco-content-common | 0.1.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| contentMediaTypeCache.enabled | bool | `true` |  |
| contentMediaTypeCache.refreshTime | string | `"0 0 * * * *"` |  |
| elasticsearch.host | string | `"elasticsearch-master"` |  |
| elasticsearch.port | int | `9200` |  |
| fullnameOverride | string | `""` |  |
| global.alfrescoRegistryPullSecrets | string | `"quay-registry-secret"` |  |
| imagePullSecrets | list | `[]` |  |
| indexName | string | `"alfresco"` |  |
| liveIndexing.content.image.pullPolicy | string | `"IfNotPresent"` |  |
| liveIndexing.content.image.repository | string | `"quay.io/alfresco/alfresco-elasticsearch-live-indexing-content"` |  |
| liveIndexing.content.image.tag | string | `"3.1.1"` |  |
| liveIndexing.content.replicaCount | int | `1` |  |
| liveIndexing.mediation.image.pullPolicy | string | `"IfNotPresent"` |  |
| liveIndexing.mediation.image.repository | string | `"quay.io/alfresco/alfresco-elasticsearch-live-indexing-mediation"` |  |
| liveIndexing.mediation.image.tag | string | `"3.1.1"` |  |
| liveIndexing.metadata.image.pullPolicy | string | `"IfNotPresent"` |  |
| liveIndexing.metadata.image.repository | string | `"quay.io/alfresco/alfresco-elasticsearch-live-indexing-metadata"` |  |
| liveIndexing.metadata.image.tag | string | `"3.1.1"` |  |
| liveIndexing.metadata.replicaCount | int | `1` |  |
| liveIndexing.path.image.pullPolicy | string | `"IfNotPresent"` |  |
| liveIndexing.path.image.repository | string | `"quay.io/alfresco/alfresco-elasticsearch-live-indexing-path"` |  |
| liveIndexing.path.image.tag | string | `"3.1.1"` |  |
| liveIndexing.path.replicaCount | int | `1` |  |
| messageBroker.password | string | `nil` | Broker password |
| messageBroker.url | string | `nil` | Broker URL formatted as per https://activemq.apache.org/failover-transport-reference |
| messageBroker.user | string | `nil` | Broker username |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| parentNameOverride | string | `""` |  |
| pathIndexingComponent.enabled | bool | `true` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| reindexing.enabled | bool | `true` |  |
| reindexing.image.pullPolicy | string | `"IfNotPresent"` |  |
| reindexing.image.repository | string | `"quay.io/alfresco/alfresco-elasticsearch-reindexing"` |  |
| reindexing.image.tag | string | `"3.1.1"` |  |
| reindexing.pathIndexingEnabled | bool | `true` |  |
| reindexing.postgresql.database | string | `"alfresco"` |  |
| reindexing.postgresql.hostname | string | `"postgresql-acs"` |  |
| reindexing.postgresql.port | int | `5432` |  |
| reindexing.postgresql.url | string | `nil` |  |
| resources.limits.memory | string | `"2048Mi"` |  |
| resources.requests.memory | string | `"256Mi"` |  |
| securityContext | object | `{}` |  |
| tolerations | list | `[]` |  |
