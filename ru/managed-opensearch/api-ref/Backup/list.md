---
editable: false
sourcePath: en/_api-ref/mdb/opensearch/api-ref/Backup/list.md
---

# Method list
Returns the list of available backups for the specified OpenSearch cluster.
 

 
## HTTP request {#https-request}
```
GET https://{{ api-host-mdb }}/managed-opensearch/v1/backups
```
 
## Query parameters {#query_params}
 
Parameter | Description
--- | ---
folderId | <p>Required. ID of the folder to list backups in.</p> <p>The maximum string length in characters is 50.</p> 
pageSize | <p>The maximum number of results per page that should be returned.</p> <p>If the number of available results is larger than <a href="/docs/managed-opensearch/api-ref/Backup/list#query_params">pageSize</a>, the service returns a <a href="/docs/managed-opensearch/api-ref/Backup/list#responses">nextPageToken</a> that can be used to get the next page of results in subsequent list requests.</p> <p>Default value is 100.</p> <p>Acceptable values are 0 to 1000, inclusive.</p> 
pageToken | <p>The page token. To get the next page of results, set <a href="/docs/managed-opensearch/api-ref/Backup/list#query_params">pageToken</a> to the <a href="/docs/managed-opensearch/api-ref/Backup/list#responses">nextPageToken</a> returned by the previous list request.</p> <p>The maximum string length in characters is 100.</p> 
 
## Response {#responses}
**HTTP Code: 200 - OK**

```json 
{
  "backups": [
    {
      "id": "string",
      "folderId": "string",
      "sourceClusterId": "string",
      "startedAt": "string",
      "createdAt": "string",
      "indices": [
        "string"
      ],
      "opensearchVersion": "string",
      "sizeBytes": "string",
      "indicesTotal": "string"
    }
  ],
  "nextPageToken": "string"
}
```

 
Field | Description
--- | ---
backups[] | **object**<br><p>Requested list of backups.</p> 
backups[].<br>id | **string**<br><p>Required. ID of the backup.</p> 
backups[].<br>folderId | **string**<br><p>ID of the folder that the backup belongs to.</p> 
backups[].<br>sourceClusterId | **string**<br><p>ID of the OpenSearch cluster that the backup was created for.</p> 
backups[].<br>startedAt | **string** (date-time)<br><p>Time when the backup operation was started.</p> <p>String in <a href="https://www.ietf.org/rfc/rfc3339.txt">RFC3339</a> text format.</p> 
backups[].<br>createdAt | **string** (date-time)<br><p>Time when the backup operation was completed.</p> <p>String in <a href="https://www.ietf.org/rfc/rfc3339.txt">RFC3339</a> text format.</p> 
backups[].<br>indices[] | **string**<br><p>Names of indices in the backup.</p> <p>The maximum number of elements is 100.</p> 
backups[].<br>opensearchVersion | **string**<br><p>OpenSearch version used to create the backup.</p> 
backups[].<br>sizeBytes | **string** (int64)<br><p>Size of the backup in bytes.</p> 
backups[].<br>indicesTotal | **string** (int64)<br><p>The number of indices in the backup.</p> 
nextPageToken | **string**<br><p>This token allows you to get the next page of results for a list request.</p> <p>If the number of results is larger than <a href="/docs/managed-opensearch/api-ref/Backup/list#query_params">pageSize</a> specified in the request, use the <a href="/docs/managed-opensearch/api-ref/Backup/list#responses">nextPageToken</a> as the value for the <a href="/docs/managed-opensearch/api-ref/Backup/list#query_params">pageToken</a> parameter in the next list request.</p> <p>Each subsequent ListBackups request has its own <a href="/docs/managed-opensearch/api-ref/Backup/list#responses">nextPageToken</a> to continue paging through the results.</p> 