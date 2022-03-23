# MFHD records transformation results   
Time Finished: 2022-03-21T11:16:01.094884   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## Record status (leader pos 5)    
Library action: **Consider fixing d-values before migration**<br/>An overview of the Record statuses (Leader position 5) present in your source data.    Pay attention to the number of occurrences of the value 'd'. These d's are expressing that they are deleted, and the records might not work as expected in FOLIO. Consider marking them as suppressed in your current system and export them as a separate batch in order to have them suppressed in FOLIO. Allowed values according to the MARC standard are a,c,d,n,p    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
n | 4   
</details>   
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
Holdings records written to disk | 4   
SRS records written to disk | 4   
Total number of Tags processed | 20   
</details>   
   
## Callnumber type mapping    
Call number types in MFHDs are mapped from 852, Indicator 1 according to a certain scheme. (LOC documentation)[https://www.loc.gov/marc/holdings/hd852.html]    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Mapped from Indicator 1 0 -> Library of Congress classification | 4   
</details>   
   
## Exceptions    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
set_location_id_by_code condition used in rules. Deprecated condition. Switch to set_permanent_location_id | 4   
</details>   
   
## Location mapping    
These are the results for the mapping between legacy locations and your new FOLIO location structure    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
'cd' (maps,cd) -> maps cd | 1   
'infoOff' (InfoOff) -> Client Services Offices | 1   
'jnlDesk' (JnlDesk) -> JOURNALS/REFERENCE DESK | 1   
'maps' (maps,cd) -> maps cd | 1   
</details>   
   
## Incomplete entity mapping adding entity    
**NO ACTION REQUIRED** <br/>This is a coding anomaly that FSE will look into.  <br/>Usually, the library does not have to do anything about it.<br/> One thing to look at is if there are many repeated subfields or unexpected patterns of subfields in the table.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
852 b:has_value - h:has_value - i:has_value ->>-->> notes note:'False' - holdingsNoteTypeId:'False' - staffOnly:'True'   | 8   
</details>   
   
## Holdings type mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
x -> Monograph -> Monograph (03c9c400-b9e3-4a07-ac0e-05ab470233ed | 4   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 4  
acquisitionFormat | 0 (0%) | 4  
acquisitionMethod | 0 (0%) | 4  
administrativeNotes | 0 (0%) | 4  
bareHoldingsItems | 0 (0%) | 4  
callNumber | 4 (100%) | 0  
callNumberPrefix | 0 (0%) | 4  
callNumberSuffix | 0 (0%) | 4  
callNumberTypeId | 4 (100%) | 0  
copyNumber | 0 (0%) | 4  
digitizationPolicy | 0 (0%) | 4  
discoverySuppress | 0 (0%) | 4  
effectiveLocationId | 0 (0%) | 4  
electronicAccess | 0 (0%) | 4  
holdingsInstance | 0 (0%) | 4  
holdingsItems | 0 (0%) | 4  
holdingsTypeId | 4 (100%) | 0  
hrid | 0 (0%) | 4  
id | 4 (100%) | 0  
illPolicy | 0 (0%) | 4  
illPolicyId | 0 (0%) | 4  
instanceId | 4 (100%) | 0  
metadata.createdByUserId | 4 (100%) | 0  
metadata.createdDate | 4 (100%) | 0  
metadata.updatedByUserId | 4 (100%) | 0  
metadata.updatedDate | 4 (100%) | 0  
notes | 0 (0%) | 4  
numberOfItems | 0 (0%) | 4  
permanentLocation | 0 (0%) | 4  
permanentLocationId | 4 (100%) | 0  
receiptStatus | 0 (0%) | 4  
receivingHistory | 0 (0%) | 4  
retentionPolicy | 0 (0%) | 4  
shelvingTitle | 0 (0%) | 4  
sourceId | 0 (0%) | 4  
statisticalCodeIds | 0 (0%) | 4  
tags | 0 (0%) | 4  
temporaryLocationId | 0 (0%) | 4  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
001 | 4 (100.0%) | 4 (100%) | 0  
004 | 4 (100.0%) | 4 (100%) | 0  
005 | 4 (100.0%) | 0 (0%) | 4  
008 | 4 (100.0%) | 0 (0%) | 4  
852 | 4 (100.0%) | 4 (100%) | 0  
</details>   
