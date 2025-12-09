## ArchiveReady
![imsdb_archiveready](https://github.com/Oksceg/archives25/blob/main/imsdb/imsdb_archiveready.png)

Достаточно высокие результаты практически по всем параметрам. Хуже всего выглядит результат по доступности (Accessibility): показатель меньше 50%

Посмотрим более подробно на анализ данных через Metawarc:


## Metawarc
### Команда analyze 
Результаты оформлены в таблице

```
metawarc analyze imsdb.com.warc.gz
2025-12-09 03:03:42,732 - root - DEBUG - Preparing imsdb.com.warc.gz
```
| mimes  | files | size  | share |
| ------------- |:-------------:|:-------------:|:-------------:|
| text/html      | 6674     |372817830 |  95.875
| image/jpeg      | 1277     |15882153  |  4.0843
| image/gif      | 30     |154576  |  0.0397512
| text/css      | 1     |2953  |  0.000759403
| application/javascript      | 1     |706  |  0.000181557
| #total        | 7983     |388858218 | 100


### Команда index

```
metawarc index imsdb.com.warc.gz
2025-12-09 15:20:58,834 - root - DEBUG - Indexing imsdb.com.warc.gz
CDX file found. Estimated number of WARC records 7983
Processed 250 (3.13%) records
Processed 500 (6.26%) records
Processed 750 (9.39%) records
Processed 1000 (12.53%) records
Processed 1250 (15.66%) records
Processed 1500 (18.79%) records
Processed 1750 (21.92%) records
Processed 2000 (25.05%) records
Processed 2250 (28.18%) records
Processed 2500 (31.32%) records
Processed 2750 (34.45%) records
Processed 3000 (37.58%) records
Processed 3250 (40.71%) records
Processed 3500 (43.84%) records
Processed 3750 (46.97%) records
Processed 4000 (50.11%) records
Processed 4250 (53.24%) records
Processed 4500 (56.37%) records
Processed 4750 (59.50%) records
Processed 5000 (62.63%) records
Processed 5250 (65.76%) records
Processed 5500 (68.90%) records
Processed 5750 (72.03%) records
Processed 6000 (75.16%) records
Processed 6250 (78.29%) records
Processed 6500 (81.42%) records
Processed 6750 (84.55%) records
Processed 7000 (87.69%) records
Processed 7250 (90.82%) records
Processed 7500 (93.95%) records
Processed 7750 (97.08%) records
```

### Команда metadata 
```
metawarc metadata --filetypes pdf --output imsdb.com_meta.jsonl imsdb.com.warc.gz
```

Результат в imsdb.com_meta.jsonl
