These are backup copies of the same files used in Lab1 incase the storage account listed in the lab is unavailable or files missing.

First one-time ingesiton URI for blob container via [OneClick UI](https://dataexplorer.azure.com/oneclick).
```url
https://adxsamplefiles.blob.core.windows.net/publiccsvsamples/logsbenchmark-onegb/2014
```

Seecond ingestion of 5 blobs asyncronously to feed derived table `ingestionLogs` from source table `rawLogs` via Update Policy.
```kql
.execute database script <|
.ingest async into table logsRaw (h'https://adxsamplefiles.blob.core.windows.net/publiccsvsamples/logsbenchmark-onegb/2014/03/08/00/data.csv.gz') with (format='csv', creationTime='2024-03-08T00:00:00Z');
.ingest async into table logsRaw (h'https://adxsamplefiles.blob.core.windows.net/publiccsvsamples/logsbenchmark-onegb/2014/03/08/01/data.csv.gz') with (format='csv', creationTime='2024-03-08T01:00:00Z');
.ingest async into table logsRaw (h'https://adxsamplefiles.blob.core.windows.net/publiccsvsamples/logsbenchmark-onegb/2014/03/08/02/data.csv.gz') with (format='csv', creationTime='2024-03-08T02:00:00Z');
.ingest async into table logsRaw (h'https://adxsamplefiles.blob.core.windows.net/publiccsvsamples/logsbenchmark-onegb/2014/03/08/03/data.csv.gz') with (format='csv', creationTime='2024-03-08T03:00:00Z');
.ingest async into table logsRaw (h'https://adxsamplefiles.blob.core.windows.net/publiccsvsamples/logsbenchmark-onegb/2014/03/08/04/data.csv.gz') with (format='csv', creationTime='2024-03-08T04:00:00Z');
```
