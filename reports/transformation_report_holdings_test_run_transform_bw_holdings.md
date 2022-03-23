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
Number of bib records referenced in item: 2 | 9   
</details>   
   
## Location mapping    
These are the results for the mapping between legacy locations and your new FOLIO location structure    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
locations mapping - jnlDesk   -> JnlDesk | 6   
locations mapping - jnlDesk -> JnlDesk | 2   
locations mapping - maps   -> maps,cd | 2   
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
_version | 0 (0%) | 10  
acquisitionFormat | 0 (0%) | 10  
acquisitionMethod | 0 (0%) | 10  
administrativeNotes | 0 (0%) | 10  
bareHoldingsItems | 0 (0%) | 10  
callNumber | 0 (0%) | 10  
callNumberPrefix | 0 (0%) | 10  
callNumberSuffix | 0 (0%) | 10  
callNumberTypeId | 0 (0%) | 10  
copyNumber | 0 (0%) | 10  
digitizationPolicy | 0 (0%) | 10  
discoverySuppress | 0 (0%) | 10  
effectiveLocationId | 0 (0%) | 10  
electronicAccess | 0 (0%) | 10  
holdingsInstance | 0 (0%) | 10  
holdingsItems | 0 (0%) | 10  
holdingsStatements | 0 (0%) | 10  
holdingsStatementsForIndexes | 0 (0%) | 10  
holdingsStatementsForSupplements | 0 (0%) | 10  
holdingsTypeId | 10 (100%) | 0  
hrid | 0 (0%) | 10  
id | 10 (100%) | 0  
illPolicy | 0 (0%) | 10  
illPolicyId | 0 (0%) | 10  
instanceId | 10 (100%) | 0  
metadata.createdByUserId | 10 (100%) | 0  
metadata.createdDate | 10 (100%) | 0  
metadata.updatedByUserId | 10 (100%) | 0  
metadata.updatedDate | 10 (100%) | 0  
notes | 0 (0%) | 10  
numberOfItems | 0 (0%) | 10  
permanentLocation | 0 (0%) | 10  
permanentLocationId | 10 (100%) | 0  
receiptStatus | 0 (0%) | 10  
receivingHistory | 0 (0%) | 10  
retentionPolicy | 0 (0%) | 10  
shelvingTitle | 0 (0%) | 10  
sourceId | 10 (100%) | 0  
statisticalCodeIds | 0 (0%) | 10  
tags | 0 (0%) | 10  
temporaryLocationId | 0 (0%) | 10  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
LOCATION | 10 (100.0%) | 10 (100%) | 0  
RECORD #(BIBLIO) | 20 (200.0%) | 20 (200%) | 0  
RECORD #(ITEM) | 10 (100.0%) | 10 (100%) | 0  
</details>   
