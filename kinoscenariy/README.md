## ArchiveReady
![kinoscenariy_archiveready](https://github.com/Oksceg/archives25/blob/main/kinoscenariy/kinoscenariy_archiveready.png)

## Metawarc
### Команда analyze 
Результаты оформлены в таблице

```
metawarc analyze kinoscenariy.com.warc.gz
2025-12-09 03:02:36,411 - root - DEBUG - Preparing kinoscenariy.com.warc.gz
```
| mimes  | files | size  | share |
| ------------- |:-------------:|:-------------:|:-------------:|
| text/html      | 307 | 30448524  | 50.1278
| image/jpeg      | 831 | 24986583 |  41.1358
| image/png      | 78  | 3286769  |  5.41105
| text/css      | 12     |1062089  |  1.74853
| image/gif      | 11  |  407202  |  0.670382
| application/javascript      |         5  |  160995  |  0.265048
|image/svg+xml              |          4  |  143590  |  0.236394
|application/octet-stream      |       4  |  104062  |  0.171319
|application/vnd.ms-fontobject   |     3  |   71373  |  0.117502
|font/woff           |                 3  |   47485  |  0.0781752
|text/xml            |                 1  |   22609  |  0.0372215
|text/plain          |                 1  |     473  |  0.000778707
|#total              |              1260  |60741754  |100



### Команда index

```
metawarc index kinoscenariy.com.warc.gz
2025-12-09 15:27:49,928 - root - DEBUG - Indexing kinoscenariy.com.warc.gz
CDX file found. Estimated number of WARC records 1260
Processed 250 (19.84%) records
Processed 500 (39.68%) records
Processed 750 (59.52%) records
Processed 1000 (79.37%) records
Processed 1250 (99.21%) records
```

### Команда metadata

```
metawarc metadata --filetypes pdf --output kinoscenariy.com_meta.jsonl  kinoscenariy.com.warc.gz
```
Результат в kinoscenariy.com_meta.jsonl

