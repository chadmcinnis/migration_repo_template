<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Number of Legacy items in file_name='items_linked_to_mfhds.csv' suppressed=False | 3   
Number of files processed | 1   
Number of legacy items in total | 3   
Number of records written to disk | 3   
</details>   
   
## Default values added    
The values below was added to all records from the value field in the mapping file instead of coming from the source records    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
5a15e0f8-2802-4cbf-a4de-8f0dedd3ed3a added to notes[0].itemNoteTypeId | 3   
False added to notes[0].staffOnly | 3   
</details>   
   
## Status mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
'' -> Available | 3   
</details>   
   
## Mapped Material Types    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
33 -> sound recording | 1   
42 -> video recording | 2   
</details>   
   
## Permanent Loan type mapping    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
33 -> catetest | 1   
42 -> MSU Hold Only | 2   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 3  
accessionNumber | 0 (0%) | 3  
administrativeNotes | 0 (0%) | 3  
barcode | 3 (100%) | 0  
chronology | 3 (100%) | 0  
circulationNotes | 0 (0%) | 3  
copyNumber | 3 (100%) | 0  
descriptionOfPieces | 3 (100%) | 0  
discoverySuppress | 0 (0%) | 3  
effectiveCallNumberComponents | 0 (0%) | 3  
effectiveLocationId | 0 (0%) | 3  
effectiveShelvingOrder | 0 (0%) | 3  
electronicAccess | 0 (0%) | 3  
enumeration | 3 (100%) | 0  
holdingsRecord2 | 0 (0%) | 3  
holdingsRecordId | 3 (100%) | 0  
hrid | 3 (100%) | 0  
id | 3 (100%) | 0  
inTransitDestinationServicePointId | 0 (0%) | 3  
itemDamagedStatusDate | 0 (0%) | 3  
itemDamagedStatusId | 0 (0%) | 3  
itemIdentifier | 0 (0%) | 3  
itemLevelCallNumber | 1 (33%) | 2  
itemLevelCallNumberPrefix | 0 (0%) | 3  
itemLevelCallNumberSuffix | 0 (0%) | 3  
itemLevelCallNumberTypeId | 0 (0%) | 3  
lastCheckIn | 0 (0%) | 3  
materialType | 0 (0%) | 3  
materialTypeId | 3 (100%) | 0  
metadata.createdByUserId | 3 (100%) | 0  
metadata.createdDate | 3 (100%) | 0  
metadata.updatedByUserId | 3 (100%) | 0  
metadata.updatedDate | 3 (100%) | 0  
missingPieces | 0 (0%) | 3  
missingPiecesDate | 0 (0%) | 3  
notes.itemNoteTypeId | 3 (100%) | 0  
notes.note | 3 (100%) | 0  
numberOfMissingPieces | 0 (0%) | 3  
numberOfPieces | 3 (100%) | 0  
permanentLoanTypeId | 3 (100%) | 0  
permanentLocation | 0 (0%) | 3  
permanentLocationId | 0 (0%) | 3  
purchaseOrderLineIdentifier | 0 (0%) | 3  
statisticalCodeIds | 0 (0%) | 3  
status.date | 3 (100%) | 0  
status.name | 3 (100%) | 0  
tags | 0 (0%) | 3  
temporaryLoanTypeId | 0 (0%) | 3  
temporaryLocation | 0 (0%) | 3  
temporaryLocationId | 0 (0%) | 3  
volume | 0 (0%) | 3  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
CHRON | 3 (100.0%) | 3 (100%) | 0  
COPY_NUMBER | 3 (100.0%) | 3 (100%) | 0  
ITEM_BARCODE | 3 (100.0%) | 3 (100%) | 0  
ITEM_ENUM | 3 (100.0%) | 3 (100%) | 0  
ITEM_ID | 6 (200.0%) | 6 (200%) | 0  
ITEM_LEVEL_CALL_NUMBER | 1 (33.3%) | 1 (33%) | 0  
ITEM_TYPE_ID | 6 (200.0%) | 6 (200%) | 0  
MFHD_ID | 6 (200.0%) | 6 (200%) | 0  
PIECES | 6 (200.0%) | 6 (200%) | 0  
YEAR | 3 (100.0%) | 3 (100%) | 0  
</details>   
