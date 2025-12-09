

## Metawarc
### Команда analyze 
Результаты оформлены в таблице

```
metawarc analyze moviescriptsandscreenplays.com.warc.gz
2025-12-09 02:46:48,244 - root - DEBUG - Preparing moviescriptsandscreenplays.com.warc.gz
```
| mimes  | files | size  | share |
| ------------- |:-------------:|:-------------:|:-------------:|
| text/plain      | 33     |4776619 |  73.6586
| text/html       | 44  | 1642525  | 25.3288
|image/gif        | 8   | 55366    | 0.85378
|image/jpeg       |2    |10298    | 0.158802
|#total           |87  |6484808 | 100


### Команда index

```
metawarc index moviescriptsandscreenplays.com.warc.gz
2025-12-09 15:29:12,584 - root - DEBUG - Indexing moviescriptsandscreenplays.com.warc.gz
CDX file found. Estimated number of WARC records 87
```

### Команда metadata

```
metawarc metadata --filetypes pdf --output moviescriptsandscreenplays.com_meta.jsonl  moviescriptsandscreenplays.com.warc.gz
```
Результат в moviescriptsandscreenplays.com_meta.jsonl
