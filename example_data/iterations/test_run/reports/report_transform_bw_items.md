# Item transformation report   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
## Timings   
   
Measure | Value   
--- | ---:   
Time Started: | 2022-09-20T21:14:03.015273+00:00   
Time Finished: | 2022-09-20T21:14:07.135249+00:00   
Elapsed time: | 0:00:04.119976   
   
## General statistics    
A list of general counters to outline the transformation as a whole.    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Number of Legacy items in file_name='bw_items.tsv' suppressed=False staff_suppressed=False service_point_id='' | 10   
Number of files processed | 1   
Number of legacy items in total | 10   
Number of records written to disk | 10   
</details>   
   
## Status mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
'' -> Available | 10   
</details>   
   
## Mapped Material Types    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
a   -> sound recording | 9   
c   -> video recording | 1   
</details>   
   
## Permanent Loan type mapping    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
0 -> Can circulate | 9   
199 -> Reading room | 1   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 10  
accessionNumber | 0 (0%) | 10  
administrativeNotes | 0 (0%) | 10  
barcode | 10 (100%) | 0  
chronology | 0 (0%) | 10  
circulationNotes | 0 (0%) | 10  
copyNumber | 0 (0%) | 10  
descriptionOfPieces | 0 (0%) | 10  
discoverySuppress | 0 (0%) | 10  
effectiveCallNumberComponents | 0 (0%) | 10  
effectiveLocationId | 0 (0%) | 10  
effectiveShelvingOrder | 0 (0%) | 10  
electronicAccess | 0 (0%) | 10  
enumeration | 0 (0%) | 10  
holdingsRecord2 | 0 (0%) | 10  
holdingsRecordId | 10 (100%) | 0  
hrid | 10 (100%) | 0  
id | 10 (100%) | 0  
inTransitDestinationServicePointId | 0 (0%) | 10  
itemDamagedStatusDate | 0 (0%) | 10  
itemDamagedStatusId | 0 (0%) | 10  
itemIdentifier | 0 (0%) | 10  
itemLevelCallNumber | 0 (0%) | 10  
itemLevelCallNumberPrefix | 0 (0%) | 10  
itemLevelCallNumberSuffix | 0 (0%) | 10  
itemLevelCallNumberTypeId | 0 (0%) | 10  
lastCheckIn | 0 (0%) | 10  
materialType | 0 (0%) | 10  
materialTypeId | 10 (100%) | 0  
metadata.createdByUserId | 10 (100%) | 0  
metadata.createdDate | 10 (100%) | 0  
metadata.updatedByUserId | 10 (100%) | 0  
metadata.updatedDate | 10 (100%) | 0  
missingPieces | 0 (0%) | 10  
missingPiecesDate | 0 (0%) | 10  
notes | 0 (0%) | 10  
numberOfMissingPieces | 0 (0%) | 10  
numberOfPieces | 0 (0%) | 10  
permanentLoanTypeId | 10 (100%) | 0  
permanentLocation | 0 (0%) | 10  
permanentLocationId | 0 (0%) | 10  
purchaseOrderLineIdentifier | 0 (0%) | 10  
statisticalCodeIds | 0 (0%) | 10  
status.date | 10 (100%) | 0  
status.name | 10 (100%) | 0  
tags | 0 (0%) | 10  
temporaryLoanTypeId | 0 (0%) | 10  
temporaryLocation | 0 (0%) | 10  
temporaryLocationId | 0 (0%) | 10  
volume | 0 (0%) | 10  
yearCaption | 0 (0%) | 10  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
BARCODE(ITEM) | 10 (100.0%) | 10 (100%) | 0  
I TYPE | 10 (100.0%) | 10 (100%) | 0  
MAT TYPE | 10 (100.0%) | 10 (100%) | 0  
RECORD #(BIBLIO) | 10 (100.0%) | 10 (100%) | 0  
RECORD #(ITEM) | 30 (300.0%) | 30 (300%) | 0  
</details>   
