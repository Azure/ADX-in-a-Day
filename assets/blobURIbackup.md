These are backup copies of the same files used in Lab1 incase the storage account listed in the lab is unavailable or files missing.

First one-time ingesiton URI for blob container via [OneClick UI](https://dataexplorer.azure.com/oneclick).
```url
https://iotmonitoringsa26915.blob.core.windows.net/logsbenchmark-onegb/2014/?sv=2023-01-03&st=2024-04-04T20%3A13%3A52Z&se=2044-04-05T20%3A13%3A00Z&sr=c&sp=rl&sig=vVnjVu0oxiR2KXq1%2FMVuJX17taKBNDeUig9lRh92pLw%3D
```

Seecond ingestion of 5 blobs asyncronously to feed derived table `ingestionLogs` from source table `rawLogs` via Update Policy.
```kql
.execute database script <|
.ingest async into table logsRaw (h'https://iotmonitoringsa26915.blob.core.windows.net/logsbenchmark-onegb/2014/03/08/00/data.csv.gz?sv=2023-01-03&st=2024-04-04T20%3A13%3A52Z&se=2044-04-05T20%3A13%3A00Z&sr=c&sp=rl&sig=vVnjVu0oxiR2KXq1%2FMVuJX17taKBNDeUig9lRh92pLw%3D') with (format='csv', creationTime='2024-03-08T00:00:00Z');
.ingest async into table logsRaw (h'https://iotmonitoringsa26915.blob.core.windows.net/logsbenchmark-onegb/2014/03/08/01/data.csv.gz?sv=2023-01-03&st=2024-04-04T20%3A13%3A52Z&se=2044-04-05T20%3A13%3A00Z&sr=c&sp=rl&sig=vVnjVu0oxiR2KXq1%2FMVuJX17taKBNDeUig9lRh92pLw%3D') with (format='csv', creationTime='2024-03-08T01:00:00Z');
.ingest async into table logsRaw (h'https://iotmonitoringsa26915.blob.core.windows.net/logsbenchmark-onegb/2014/03/08/02/data.csv.gz?sv=2023-01-03&st=2024-04-04T20%3A13%3A52Z&se=2044-04-05T20%3A13%3A00Z&sr=c&sp=rl&sig=vVnjVu0oxiR2KXq1%2FMVuJX17taKBNDeUig9lRh92pLw%3D') with (format='csv', creationTime='2024-03-08T02:00:00Z');
.ingest async into table logsRaw (h'https://iotmonitoringsa26915.blob.core.windows.net/logsbenchmark-onegb/2014/03/08/03/data.csv.gz?sv=2023-01-03&st=2024-04-04T20%3A13%3A52Z&se=2044-04-05T20%3A13%3A00Z&sr=c&sp=rl&sig=vVnjVu0oxiR2KXq1%2FMVuJX17taKBNDeUig9lRh92pLw%3D') with (format='csv', creationTime='2024-03-08T03:00:00Z');
.ingest async into table logsRaw (h'https://iotmonitoringsa26915.blob.core.windows.net/logsbenchmark-onegb/2014/03/08/04/data.csv.gz?sv=2023-01-03&st=2024-04-04T20%3A13%3A52Z&se=2044-04-05T20%3A13%3A00Z&sr=c&sp=rl&sig=vVnjVu0oxiR2KXq1%2FMVuJX17taKBNDeUig9lRh92pLw%3D') with (format='csv', creationTime='2024-03-08T04:00:00Z');
```
