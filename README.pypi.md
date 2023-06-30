![Lines of code](https://img.shields.io/tokei/lines/github/ablaternae/py-csv-deta)
[![PyPI version](https://badge.fury.io/py/csv-deta.svg)](https://badge.fury.io/py/csv-deta)
![Downloads](https://img.shields.io/pypi/dm/csv-deta)
[![Statistic](https://pepy.tech/badge/csv-deta/week)](https://pepy.tech/project/csv-deta)
[![GitHub](https://img.shields.io/github/license/ablaternae/py-csv-deta)](https://github.com/ablaternae/py-csv-deta/blob/trunk/LICENSE.md)

# ALPHA version! work in progress

## Lightweight utility to upload and download CSV files data into\from Deta Base

* it's based on [csvtodeta](https://pypi.org/project/csvtodeta/) tool by [@Fredy Somy](https://github.com/fredysomy/CsvToDeta)
* improvements:
  * more options
  * upload about twice as fast ([put() method is used](https://docs.deta.sh/docs/base/sdk#using))
  * bulk load: up 25 \ down 1000 rows per iteration

### install
```bash
pip install -U csv-deta
```
### use
```bash
csv-deta upload PATH_TO_CSV_FILE [--dbname DETA_DB_NAME] [--project DETA_PROJECT_KEY] 
```
by default `DETA_DB_NAME` param will be created from `PATH_TO_CSV_FILE` filename without ext, 
and `DETA_PROJECT_KEY` -- from the same name's environment variable; 
for other options see also `csv-deta upload|download --help`

### todo
* [x] download data
* [x] upload speed optimization
* [ ] async transfer
* [ ] validate source csv (?)

----
enjoy, star it, and donate
