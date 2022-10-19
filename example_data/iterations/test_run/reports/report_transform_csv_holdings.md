# Holdings transformation report   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
## Timings   
   
Measure | Value   
--- | ---:   
Time Started: | 2022-09-20T21:13:21.127572+00:00   
Time Finished: | 2022-09-20T21:13:26.135605+00:00   
Elapsed time: | 0:00:05.008033   
   
## Holdings Merging    
    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
Duplicate key based on current merge criteria. Records merged | 1   
Previously transformed holdings record loaded | 3   
callNumber empty or not set | 3   
</details>   
   
## General statistics    
A list of general counters to outline the transformation as a whole.    
<details><summary>Click to expand all 7 things</summary>     
   
Measure | Count   
--- | ---:   
Holdings Records Written to disk | 5   
Holdings already created from Item | 1   
Number of Legacy items in file | 3   
Number of files processed | 1   
Records matched to Instances | 3   
Unique Holdings created from Items | 2   
</details>   
   
## Bound-with mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Number of bib records referenced in item: 1 | 3   
</details>   
   
## Location mapping    
These are the results for the mapping between legacy locations and your new FOLIO location structure    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
Unmapped (Default value was set) -- MAIN - ACDPM -> KU/CC/DI/2 | 2   
Unmapped (Default value was set) -- REN - ACDPM -> KU/CC/DI/2 | 1   
</details>   
   
## Default values added    
The values below was added to all records from the value field in the mapping file instead of coming from the source records    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
True added to notes[0].staffOnly | 3   
f453de0f-8b54-4e99-9180-52932529e3a6 added to notes[0].holdingsNoteTypeId | 3   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 3  
acquisitionFormat | 0 (0%) | 3  
acquisitionMethod | 0 (0%) | 3  
administrativeNotes | 0 (0%) | 3  
bareHoldingsItems | 0 (0%) | 3  
callNumber | 0 (0%) | 3  
callNumberPrefix | 0 (0%) | 3  
callNumberSuffix | 0 (0%) | 3  
callNumberTypeId | 0 (0%) | 3  
copyNumber | 0 (0%) | 3  
digitizationPolicy | 0 (0%) | 3  
discoverySuppress | 0 (0%) | 3  
effectiveLocationId | 0 (0%) | 3  
electronicAccess | 0 (0%) | 3  
holdingsInstance | 0 (0%) | 3  
holdingsItems | 0 (0%) | 3  
holdingsStatements.statement | 3 (100%) | 0  
holdingsStatementsForIndexes | 0 (0%) | 3  
holdingsStatementsForSupplements | 0 (0%) | 3  
holdingsTypeId | 3 (100%) | 0  
hrid | 0 (0%) | 3  
id | 3 (100%) | 0  
illPolicy | 0 (0%) | 3  
illPolicyId | 0 (0%) | 3  
instanceId | 3 (100%) | 0  
metadata.createdByUserId | 3 (100%) | 0  
metadata.createdDate | 3 (100%) | 0  
metadata.updatedByUserId | 3 (100%) | 0  
metadata.updatedDate | 3 (100%) | 0  
notes.holdingsNoteTypeId | 3 (100%) | 0  
notes.note | 3 (100%) | 0  
notes.staffOnly | 3 (100%) | 0  
numberOfItems | 0 (0%) | 3  
permanentLocation | 0 (0%) | 3  
permanentLocationId | 3 (100%) | 0  
receiptStatus | 0 (0%) | 3  
receivingHistory | 0 (0%) | 3  
retentionPolicy | 0 (0%) | 3  
shelvingTitle | 0 (0%) | 3  
sourceId | 3 (100%) | 0  
statisticalCodeIds | 0 (0%) | 3  
tags | 0 (0%) | 3  
temporaryLocationId | 0 (0%) | 3  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
PERM_LOCATION | 3 (100.0%) | 3 (100%) | 0  
Z30_REC_KEY | 3 (100.0%) | 3 (100%) | 0  
fake_instance_id | 3 (100.0%) | 3 (100%) | 0  
</details>   
