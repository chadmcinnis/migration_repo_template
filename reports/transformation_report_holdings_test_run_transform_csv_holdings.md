<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## Holdings Merging    
    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
Duplicate key based on current merge criteria. Records merged | 1   
Previously transformed holdings record loaded | 3   
callNumber empty or not set | 2   
</details>   
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
Holdings Records Written to disk | 5   
Number of Legacy items in file | 2   
Number of files processed | 1   
Records matched to Instances | 2   
Unique Holdings created from Items | 2   
</details>   
   
## Bound-with mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Number of bib records referenced in item: 1 | 2   
</details>   
   
## Location mapping    
These are the results for the mapping between legacy locations and your new FOLIO location structure    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
Unmapped (Default value was set) -- MAIN - ACDPM -> maps,cd | 1   
Unmapped (Default value was set) -- REN - ACDPM -> maps,cd | 1   
</details>   
   
## Default values added    
The values below was added to all records from the value field in the mapping file instead of coming from the source records    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
True added to notes[0].staffOnly | 2   
f453de0f-8b54-4e99-9180-52932529e3a6 added to notes[0].holdingsNoteTypeId | 2   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 2  
acquisitionFormat | 0 (0%) | 2  
acquisitionMethod | 0 (0%) | 2  
administrativeNotes | 0 (0%) | 2  
bareHoldingsItems | 0 (0%) | 2  
callNumber | 0 (0%) | 2  
callNumberPrefix | 0 (0%) | 2  
callNumberSuffix | 0 (0%) | 2  
callNumberTypeId | 0 (0%) | 2  
copyNumber | 0 (0%) | 2  
digitizationPolicy | 0 (0%) | 2  
discoverySuppress | 0 (0%) | 2  
effectiveLocationId | 0 (0%) | 2  
electronicAccess | 0 (0%) | 2  
holdingsInstance | 0 (0%) | 2  
holdingsItems | 0 (0%) | 2  
holdingsStatements | 0 (0%) | 2  
holdingsStatementsForIndexes | 0 (0%) | 2  
holdingsStatementsForSupplements | 0 (0%) | 2  
holdingsTypeId | 2 (100%) | 0  
hrid | 0 (0%) | 2  
id | 2 (100%) | 0  
illPolicy | 0 (0%) | 2  
illPolicyId | 0 (0%) | 2  
instanceId | 2 (100%) | 0  
metadata.createdByUserId | 2 (100%) | 0  
metadata.createdDate | 2 (100%) | 0  
metadata.updatedByUserId | 2 (100%) | 0  
metadata.updatedDate | 2 (100%) | 0  
notes.holdingsNoteTypeId | 2 (100%) | 0  
notes.note | 2 (100%) | 0  
notes.staffOnly | 2 (100%) | 0  
numberOfItems | 0 (0%) | 2  
permanentLocation | 0 (0%) | 2  
permanentLocationId | 2 (100%) | 0  
receiptStatus | 0 (0%) | 2  
receivingHistory | 0 (0%) | 2  
retentionPolicy | 0 (0%) | 2  
shelvingTitle | 0 (0%) | 2  
sourceId | 2 (100%) | 0  
statisticalCodeIds | 0 (0%) | 2  
tags | 0 (0%) | 2  
temporaryLocationId | 0 (0%) | 2  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
PERM_LOCATION | 2 (100.0%) | 2 (100%) | 0  
Z30_REC_KEY | 2 (100.0%) | 2 (100%) | 0  
fake_instance_id | 2 (100.0%) | 2 (100%) | 0  
</details>   
