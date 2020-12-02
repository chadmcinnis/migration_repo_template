# Migration Repo template
This repo is a template repository for the files needed for migrating Inventory data from a source system into FOLIO 
In order to perform migrations according to this process, you need to clone the following repositories:   
* [MARC21-to-FOLIO](https://github.com/FOLIO-FSE/MARC21-To-FOLIO)
* [service_tools](https://github.com/FOLIO-FSE/service_tools)

# Mapping files
The repo contains the following mapping files in the Mapping files folder.

# What file is needed for what objects?
File\Process | Bibs->Instances | Holdings | Items 
------------ | ------------- | ------------- | -------------
marc-instance-mapping-rules.json  | yes | no | no
mfhd_rules.json  | no | yes | no
item_to_item.json  | no | no | yes
locations.tsv  | no | yes | yes
material_types.tsv  | no | no | yes
loan_types.tsv  | yes | no | yes

## marc-instance-mapping-rules.json
These are the mapping rules from MARC21 bib records to FOLIO instances. The rules are stored in the tenant, but it is good practice to keep them under version control so you can maintain the customizations as the mapping rules evolve.For more information on syntax etc, read the [documentation](https://github.com/folio-org/mod-source-record-manager/blob/master/RuleProcessorApi.md).

## mfhd_rules.json
This file is built out according to the [mapping rules for bibs](https://github.com/folio-org/mod-source-record-manager/blob/master/RuleProcessorApi.md). The conditions are different, and not well documented at this point. Look at the example file and refer to the mappinrules documentation 


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

## locations.tsv
These are the mappings of the legacy and FOLIO locations. The file is structured like this:
 legacy_code | folio_code 
------------ | ------------- 
 AFAS | AFA
 
The file is needed for both Holdings migration and Item migration

## material_types.tsv
These mappings can be more complex. The first column name is fixed, since that is the target material type in FOLIO. Then you add the column names from the Item export TSV. For each column added, the values in them must match. At least one value per column must match. Se loan_types.tsv for complex examples
 folio_name | Z30_MATERIAL 
------------ | ------------- 
 Audiocassette | ACASS

## loan_types.tsv
These mappings can be more complex. The first column name is fixed, since that is the target loan type in FOLIO. Then you add the column names from the Item export TSV. For each column added, the values in them must match. At least one value per column must match

 folio_name | Z30_SUB_LIBRARY | Z30_ITEM_STATUS 
------------ | ------------- | -------------
 Non-circulating | UMDUB, UMSCI, UMFAC, UMSCA, UMFCD, UMIMA | 02, 03, 13

# Example Records
In the example records folder, you will find example source records and example results from after a transformation
