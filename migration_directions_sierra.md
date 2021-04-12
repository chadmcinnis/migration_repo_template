# Data migration directions for Template Library

## Contents
* [What we will migrate](#what-we-will-migrate)
* [Data to extract](#data-to-extract)
  * [Bib records](#bib-records)
  * [Serials check-in records](#serials-check-in-records)
  * [Item records](#item-records)
  * [Patron records](#patron-records)
  * [Open loans](#bib-records)
  * [Open requests](open-requests)

## What we will migrate
- Sierra bibs ➡️ FOLIO instances (scripted)
- Sierra check-in ➡️ FOLIO holdings (scripted)
- Sierra items ➡️ FOLIO holdings (scripted)
- Sierra items ➡️ FOLIO items (scripted)
- Sierra patrons ➡️ FOLIO users (scripted)
- Sierra loans ➡️ FOLIO loans (scripted)
- Sierra requests ➡️ FOLIO requests (manual)

## Data to extract
### Bib records
**Library** exports a file of .b records in MARC21 format, using Create lists and Data Exchange.

**IC** and **library** verify that the library's MARC-to-FOLIO mapping is up-to-date and correct.

### Serials check-in records
**Library** exports a file of .c records in MARC21 format, using Create lists and Data Exchange.

**IC** and **library** verify that all relevant [mapping_files](mapping_files) are up-to-date and correct.

### Item records
**IC** exports a file of .i records in json format using the Sierra APIs.

After exporting the data, **IC** will
- Transform the items into FOLIO holdings and items
- Load the holdings and items into FOLIO

**IC** and **library** verify that all relevant [mapping_files](mapping_files) are up-to-date and correct.

### Patron records
**Library** exports a file of .p records using Create lists. 

|Sierra fields to export|
|---|
|Name|
|Barcode|
|Email|
|Patron Type|
|Telephone|
|Student ID|
|Record Number|

**IC** and **library** verify that all relevant [mapping_files](mapping_files) are up-to-date and correct.

After receiving the data, **IC** will
- Split names into firstname & last name
- Transform the patrons into FOLIO users
- Load the users into FOLIO

### Open loans
**Library** exports a file of .i records using Create lists. 

|Sierra fields to export|
|---|
|BARCODE(ITEM)|
|OUT DATE|
|DUE DATE|
|TOTAL RENEWALS|
|BARCODE(PATRON)|

**Library** indicates which service point should be used as "Check out service point".

After receiving the data, **IC** will
- Transform the item data into FOLIO loans
- Load the loans into FOLIO

### Open requests
We expect the number of open requests to be so low that the migration will most easily be done manually by **library**.
