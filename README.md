# Migration Repo template
This repo is a template repository for the files needed for migrating Inventory data from a source system into FOLIO 
In order to perform migrations according to this process, you need to clone the following repositories:   
* [MARC21-to-FOLIO](https://github.com/FOLIO-FSE/MARC21-To-FOLIO)
* [service_tools](https://github.com/FOLIO-FSE/service_tools)

# Mapping files
The repo contains the following mapping files in the Mapping files folder.
## item_to_item.json
This is a mapping file for the items. The process assumes you have the item data in a CSV/TSV format. 
The structure of the file is dependant on the the column names in the TSV file. For example, if you have a file that looks like this:
... | Z30_BARCODE | Z30_CALL_NO | ... 
------------ | ------------- | ------------- | -------------
 ... | 123456790 | Some call number | ...
 


Your map should look like this:
```
...
"Z30_BARCODE": {
 	"description": "",
	"target": "barcode"
},
"Z30_CALL_NO": {
	"description": "",
	"target": "itemLevelCallNumber"
},
...
```
The resulting FOLIO Item would look like this:
```
{
	...
	"barcode": "123456790",
	"itemLevelCallNumber": "Z30_CALL_NO"
	...
}
```
### Default fields
There are a couple of properties in the file that are used for giving default values if reference data mapping fails.
There are other fields to help with other file format than TSV as well.
```
	"itemsFileDelimiter": "",
    "defaultLoantypeName": "Migration-technical",
    "defaultLocationCode": "tech",
    "defaultMaterialTypeName": "unspecified",
    "itemsFileType": "TSV",
    "legacyFieldsToCountValuesFor": [
        "Z30_ITEM_STATUS"
    ],
    "legacyIdField": "Z30_BARCODE",
    "mapOnLocationField": "code"
```
## mfhd_rules.json
This file is built out according to the [mapping rules for bibs](https://github.com/folio-org/mod-source-record-manager/blob/master/RuleProcessorApi.md). The conditions are different, and not well documented at this point. Look at the example file and refer to the mappinrules documentation 


