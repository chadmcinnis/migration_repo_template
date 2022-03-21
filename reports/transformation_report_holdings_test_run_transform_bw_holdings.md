<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 11 things</summary>     
   
Measure | Count   
--- | ---:   
BW Items found tied to previously created BW Holdings | 2   
Bib ids referenced in bound-with items | 20   
Bound-with holdings created | 20   
Bound-with items identified by bib id | 10   
Holdings Records Written to disk | 19   
Number of Legacy items in file | 11   
Number of files processed | 1   
Records matched to Instances | 21   
Unique BW Holdings created from Items | 18   
Unique Holdings created from Items | 1   
</details>   
   
## Bound-with mapping    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
Number of bib records referenced in item: 1 | 1   
Number of bib records referenced in item: 2 | 10   
</details>   
   
## Location mapping    
These are the results for the mapping between legacy locations and your new FOLIO location structure    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
locations mapping - jnlDesk   -> JnlDesk | 6   
locations mapping - jnlDesk -> JnlDesk | 2   
locations mapping - maps   -> JnlDesk | 3   
</details>   
   
## Default values added    
The values below was added to all records from the value field in the mapping file instead of coming from the source records    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
97fbb130-beb4-4eec-84a6-c69768ca3eea added to notes[0].holdingsNoteTypeId | 11   
true added to notes[0].staffOnly | 11   
</details>   
   
## Holdings Merging    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
callNumber empty or not set | 1   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 11  
acquisitionFormat | 0 (0%) | 11  
acquisitionMethod | 0 (0%) | 11  
administrativeNotes | 0 (0%) | 11  
bareHoldingsItems | 0 (0%) | 11  
callNumber | 0 (0%) | 11  
callNumberPrefix | 0 (0%) | 11  
callNumberSuffix | 0 (0%) | 11  
callNumberTypeId | 0 (0%) | 11  
copyNumber | 0 (0%) | 11  
digitizationPolicy | 0 (0%) | 11  
discoverySuppress | 0 (0%) | 11  
effectiveLocationId | 0 (0%) | 11  
electronicAccess | 0 (0%) | 11  
holdingsInstance | 0 (0%) | 11  
holdingsItems | 0 (0%) | 11  
holdingsStatements | 0 (0%) | 11  
holdingsStatementsForIndexes | 0 (0%) | 11  
holdingsStatementsForSupplements | 0 (0%) | 11  
holdingsTypeId | 11 (100%) | 0  
hrid | 0 (0%) | 11  
id | 11 (100%) | 0  
illPolicy | 0 (0%) | 11  
illPolicyId | 0 (0%) | 11  
instanceId | 11 (100%) | 0  
metadata.createdByUserId | 11 (100%) | 0  
metadata.createdDate | 11 (100%) | 0  
metadata.updatedByUserId | 11 (100%) | 0  
metadata.updatedDate | 11 (100%) | 0  
notes.holdingsNoteTypeId | 11 (100%) | 0  
notes.note | 11 (100%) | 0  
notes.staffOnly | 11 (100%) | 0  
numberOfItems | 0 (0%) | 11  
permanentLocation | 0 (0%) | 11  
permanentLocationId | 11 (100%) | 0  
receiptStatus | 0 (0%) | 11  
receivingHistory | 0 (0%) | 11  
retentionPolicy | 0 (0%) | 11  
shelvingTitle | 0 (0%) | 11  
sourceId | 0 (0%) | 11  
statisticalCodeIds | 0 (0%) | 11  
tags | 0 (0%) | 11  
temporaryLocationId | 0 (0%) | 11  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
LOCATION | 11 (100.0%) | 11 (100%) | 0  
RECORD #(BIBLIO) | 22 (200.0%) | 22 (200%) | 0  
RECORD #(ITEM) | 11 (100.0%) | 11 (100%) | 0  
</details>   
