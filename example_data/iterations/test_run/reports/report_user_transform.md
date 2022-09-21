# Users transformation report   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
## Timings   
   
Measure | Value   
--- | ---:   
Time Started: | 2022-09-20T21:14:33.914810+00:00   
Time Finished: | 2022-09-20T21:14:38.056221+00:00   
Elapsed time: | 0:00:04.141411   
   
## User group mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
STAF -> staff | 1   
</details>   
   
## Details    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
['HOMEADDRESS2', 'HOMEADDRESS3'] concatenated into one string | 1   
</details>   
   
## Default values added    
The values below was added to all records from the value field in the mapping file instead of coming from the source records    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
True added to personal.addresses.primaryAddress | 1   
</details>   
   
## General statistics    
A list of general counters to outline the transformation as a whole.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Successful user transformations | 1   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
active | 1 (100%) | 0  
barcode | 1 (100%) | 0  
externalSystemId | 1 (100%) | 0  
id | 1 (100%) | 0  
patronGroup | 1 (100%) | 0  
personal.addresses | 1 (100%) | 0  
personal.dateOfBirth | 1 (100%) | 0  
personal.email | 1 (100%) | 0  
personal.firstName | 1 (100%) | 0  
personal.lastName | 1 (100%) | 0  
personal.middleName | 1 (100%) | 0  
personal.mobilePhone | 1 (100%) | 0  
personal.phone | 1 (100%) | 0  
personal.preferredContactTypeId | 1 (100%) | 0  
requestPreference.delivery | 1 (100%) | 0  
requestPreference.holdShelf | 1 (100%) | 0  
requestPreference.metadata.createdByUserId | 1 (100%) | 0  
requestPreference.metadata.createdDate | 1 (100%) | 0  
requestPreference.metadata.updatedByUserId | 1 (100%) | 0  
requestPreference.metadata.updatedDate | 1 (100%) | 0  
requestPreference.userId | 1 (100%) | 0  
username | 1 (100%) | 0  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
BARCODE | 1 (100.0%) | 1 (100%) | 0  
EMAIL | 1 (100.0%) | 1 (100%) | 0  
FACSTAFFDATE | 1 (100.0%) | 1 (100%) | 0  
FIRSTNAME | 1 (100.0%) | 1 (100%) | 0  
HOMEADDRESS1 | 1 (100.0%) | 1 (100%) | 0  
HOMEADDRESS2 | 1 (100.0%) | 1 (100%) | 0  
HOMEADDRESS3 | 1 (100.0%) | 1 (100%) | 0  
HOMECITY | 1 (100.0%) | 1 (100%) | 0  
HOMESTATE | 1 (100.0%) | 1 (100%) | 0  
HOMEZIP | 1 (100.0%) | 1 (100%) | 0  
LASTNAME | 1 (100.0%) | 1 (100%) | 0  
MIDDLE | 1 (100.0%) | 1 (100%) | 0  
MOBILEPHONE | 1 (100.0%) | 1 (100%) | 0  
NOTE_CONTENT | 1 (100.0%) | 1 (100%) | 0  
NOTE_TITLE | 1 (100.0%) | 1 (100%) | 0  
PATRONID | 1 (100.0%) | 1 (100%) | 0  
PHONE | 1 (100.0%) | 1 (100%) | 0  
TYPE | 1 (100.0%) | 1 (100%) | 0  
USERNAME | 1 (100.0%) | 1 (100%) | 0  
some_other_note | 1 (100.0%) | 1 (100%) | 0  
some_other_note_title | 1 (100.0%) | 1 (100%) | 0  
third_note_content | 1 (100.0%) | 0 (0%) | 1  
third_note_title | 1 (100.0%) | 1 (100%) | 0  
</details>   
