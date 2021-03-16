# Migration Repo template
This repo is a template repository for the files needed for migrating Inventory data from a source system into FOLIO 

# FOLIO Inventory data migration process
This template plays a vital part in a process together with other repos allowing you to perform bibliographic data migration from a legacy ILS into FOLIO. For more information on the process, head over to the linked repos below.
In order to perform migrations according to this process, you need to clone the following repositories:   
* [MARC21-to-FOLIO](https://github.com/FOLIO-FSE/MARC21-To-FOLIO)
* [service_tools](https://github.com/FOLIO-FSE/service_tools)
* [migration_repo_template](https://github.com/FOLIO-FSE/migration_repo_template)


# Mapping files
The repo contains the following mapping files in the Mapping files folder.
There is a web tool that helps you crate the mappin files for certain objects available at https://data-mapping-file-creator.folio.ebsco.com/data_mapping_creation

## What file is needed for what objects?
File\Process | Bibs->Instances | Holdings | Items 
------------ | ------------- | ------------- | -------------
marc-instance-mapping-rules.json  | yes | no | no
mfhd_rules.json  | no | yes | no
item_mapping.json  | no | no | yes
locations.tsv  | no | yes | yes
material_types.tsv  | no | no | yes
loan_types.tsv  | no | no | yes

## marc-instance-mapping-rules.json
These are the mapping rules from MARC21 bib records to FOLIO instances. The rules are stored in the tenant, but it is good practice to keep them under version control so you can maintain the customizations as the mapping rules evolve.For more information on syntax etc, read the [documentation](https://github.com/folio-org/mod-source-record-manager/blob/master/RuleProcessorApi.md).

## mfhd_rules.json
This file is built out according to the [mapping rules for bibs](https://github.com/folio-org/mod-source-record-manager/blob/master/RuleProcessorApi.md). The conditions are different, and not well documented at this point. Look at the example file and refer to the mappinrules documentation 


## item_to_item.json
This is a mapping file for the items. The process assumes you have the item data in a CSV/TSV format. 
The structure of the file is dependant on the the column names in the TSV file. For example, if you have a file that looks like this:
... | Z30_BARCODE | Z30_CALL_NO | Z30_DESCRIPTION |  ... 
------------ | ------------- | ------------- | ------------- | -------------
 ... | 123456790 | Some call number | some note  | ...
 


Your map should look like this:
```
...
{
    "folio_field": "barcode",
    "legacy_field": "Z30_BARCODE",
    "value":"",
    "description": ""
},
{
    "folio_field": "itemLevelCallNumber",
    "legacy_field": "Z30_CALL_NO",
    "value":"",
    "description": ""
}, 
{
    "folio_field": "notes[0].itemNoteTypeId",
    "legacy_field": "Z30_DESCRIPTION",
    "value": "c7bc292c-a318-43d3-9b03-7a40dfba046a",
    "description": ""
},
{
    "folio_field": "notes[0].staffOnly",
    "legacy_field": "Z30_DESCRIPTION",
    "value": false,
    "description": ""
},
{
    "folio_field": "notes[0].note",
    "legacy_field": "Z30_DESCRIPTION",
    "value": false,
    "description": ""
},
...
```
The resulting FOLIO Item would look like this:
```
{
	...
	"barcode": "123456790",
	"itemLevelCallNumber": "Some call number"
	"notes":[{
			"staffOnly": false,
			"note": "some note",
			"itemNoteTypeId": "c7bc292c-a318-43d3-9b03-7a40dfba046a"			
		}],
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
These mappings allow for some complexity. These are the mappings of the legacy and FOLIO locations. The file must be structured like this:
 legacy_code | folio_code | Z30_COLLECTION 
------------ | ------------- | -------------
 AFAS | AFA | AFAS
 
The legacy_code part is needed for both Holdings migratiom. For Item migration, the source fields can be used (Z30_COLLECTION in this case). You can add as many source fields as you like for the Items

## material_types.tsv
These mappings allow for some complexity. The first column name is fixed, since that is the target material type in FOLIO. Then you add the column names from the Item export TSV. For each column added, the values in them must match. At least one value per column must match. Se loan_types.tsv for complex examples
 folio_name | Z30_MATERIAL 
------------ | ------------- 
 Audiocassette | ACASS

## loan_types.tsv
These mappings allow for some complexity. The first column name is fixed, since that is the target loan type in FOLIO. Then you add the column names from the Item export TSV. For each column added, the values in them must match. At least one value per column must match

 folio_name | Z30_SUB_LIBRARY | Z30_ITEM_STATUS 
------------ | ------------- | -------------
 Non-circulating | UMDUB, UMSCI, UMFAC, UMSCA, UMFCD, UMIMA | 02, 03, 13

# Example Records
In the [example records folder](https://github.com/FOLIO-FSE/migration_repo_template/tree/main/example_files), you will find example source records and example results from after a transformation
## Result files
The following table outlines the result records and their use and role
 File | Content | Use for 
------------ | ------------- | ------------- 
folio_holdings.json | FOLIO Holdings records in json format. One per row in the file | To be loaded into FOLIO using the batch APIs
folio_instances.json | FOLIO Instance records in json format. One per row in the file | To be loaded into FOLIO using the batch APIs
folio_items.json |FOLIO Item records in json format. One per row in the file | To be loaded into FOLIO using the batch APIs
holdings_id_map.json | A json map from legacy Holdings Id to the ID of the created FOLIO Holdings record | To be used in subsequent transformation steps 
holdings_transformation_report.md | A file containing various breakdowns of the transformation. Also contains errors to be fixed by the library | Create list of cleaning tasks, mapping refinement
instance_id_map.json | A json map from legacy Bib Id to the ID of the created FOLIO Instance record. Relies on the "ILS Flavour" parameter in the main_bibs.py scripts | To be used in subsequent transformation steps 
instance_transformation_report.md | A file containing various breakdowns of the transformation. Also contains errors to be fixed by the library | Create list of cleaning tasks, mapping refinement
item_id_map.json | A json map from legacy Item Id to the ID of the created FOLIO Item record | To be used in subsequent transformation steps 
item_transform_errors.tsv | A TSV file with errors and data issues together with the row number or id for the Item | To be used in fixing of data issues 
items_transformation_report.md | A file containing various breakdowns of the transformation. Also contains errors to be fixed by the library | Create list of cleaning tasks, mapping refinement
marc_xml_dump.xml | A MARCXML dump of the bib records, with the proper 001:s and 999 fields added | For pre-loading a Discovery system.
srs.json | FOLIO SRS records in json format. One per row in the file | To be loaded into FOLIO using the batch APIs

