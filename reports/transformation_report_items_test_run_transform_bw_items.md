<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Number of Legacy items in file_name='bw_items.tsv' suppressed=False | 11   
Number of files processed | 1   
Number of legacy items in total | 11   
Number of records written to disk | 11   
</details>   
   
## Status mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
'' -> Available | 11   
</details>   
   
## Mapped Material Types    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
mtypes mapping - a   -> sound recording | 10   
mtypes mapping - c   -> video recording | 1   
</details>   
   
## Permanent Loan type mapping    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
loantypes mapping - 0 -> MSU Hold Only | 10   
loantypes mapping - 199 -> MSU Hold Only | 1   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 11  
accessionNumber | 0 (0%) | 11  
administrativeNotes | 0 (0%) | 11  
barcode | 11 (100%) | 0  
chronology | 0 (0%) | 11  
circulationNotes | 0 (0%) | 11  
circulationNotes.id | 4 (36%) | 7  
circulationNotes.note | 4 (36%) | 7  
circulationNotes.source.id | 4 (36%) | 7  
circulationNotes.source.personal.firstName | 4 (36%) | 7  
circulationNotes.source.personal.lastName | 4 (36%) | 7  
copyNumber | 0 (0%) | 11  
descriptionOfPieces | 0 (0%) | 11  
discoverySuppress | 0 (0%) | 11  
effectiveCallNumberComponents | 0 (0%) | 11  
effectiveLocationId | 0 (0%) | 11  
effectiveShelvingOrder | 0 (0%) | 11  
electronicAccess | 0 (0%) | 11  
enumeration | 0 (0%) | 11  
holdingsRecord2 | 0 (0%) | 11  
holdingsRecordId | 11 (100%) | 0  
hrid | 11 (100%) | 0  
id | 11 (100%) | 0  
inTransitDestinationServicePointId | 0 (0%) | 11  
itemDamagedStatusDate | 0 (0%) | 11  
itemDamagedStatusId | 0 (0%) | 11  
itemIdentifier | 0 (0%) | 11  
itemLevelCallNumber | 0 (0%) | 11  
itemLevelCallNumberPrefix | 0 (0%) | 11  
itemLevelCallNumberSuffix | 0 (0%) | 11  
itemLevelCallNumberTypeId | 0 (0%) | 11  
lastCheckIn | 0 (0%) | 11  
materialType | 0 (0%) | 11  
materialTypeId | 11 (100%) | 0  
metadata.createdByUserId | 11 (100%) | 0  
metadata.createdDate | 11 (100%) | 0  
metadata.updatedByUserId | 11 (100%) | 0  
metadata.updatedDate | 11 (100%) | 0  
missingPieces | 0 (0%) | 11  
missingPiecesDate | 0 (0%) | 11  
notes | 0 (0%) | 11  
numberOfMissingPieces | 0 (0%) | 11  
numberOfPieces | 0 (0%) | 11  
permanentLoanTypeId | 11 (100%) | 0  
permanentLocation | 0 (0%) | 11  
permanentLocationId | 0 (0%) | 11  
purchaseOrderLineIdentifier | 0 (0%) | 11  
statisticalCodeIds | 0 (0%) | 11  
status.date | 11 (100%) | 0  
status.name | 11 (100%) | 0  
tags | 0 (0%) | 11  
temporaryLoanTypeId | 0 (0%) | 11  
temporaryLocation | 0 (0%) | 11  
temporaryLocationId | 0 (0%) | 11  
volume | 0 (0%) | 11  
yearCaption | 0 (0%) | 11  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
BARCODE(ITEM) | 11 (100.0%) | 11 (100%) | 0  
I TYPE | 11 (100.0%) | 11 (100%) | 0  
MAT TYPE | 11 (100.0%) | 11 (100%) | 0  
RECORD #(BIBLIO) | 11 (100.0%) | 11 (100%) | 0  
RECORD #(ITEM) | 33 (300.0%) | 33 (300%) | 0  
</details>   
