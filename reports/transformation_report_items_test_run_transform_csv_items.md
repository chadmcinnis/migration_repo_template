<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Number of Legacy items in file_name='csv_items.tsv' suppressed=False | 2   
Number of files processed | 1   
Number of legacy items in total | 2   
Number of records written to disk | 2   
</details>   
   
## Default values added    
The values below was added to all records from the value field in the mapping file instead of coming from the source records    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
5a15e0f8-2802-4cbf-a4de-8f0dedd3ed3a added to notes[0].itemNoteTypeId | 2   
False added to notes[0].staffOnly | 2   
</details>   
   
## Status mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
'' -> Available | 2   
</details>   
   
## Mapped Material Types    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
mtypes mapping - BOOK -> sound recording | 2   
</details>   
   
## Permanent Loan type mapping    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
loantypes mapping - BOOK -> MSU Hold Only | 2   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 2  
accessionNumber | 0 (0%) | 2  
administrativeNotes | 0 (0%) | 2  
barcode | 2 (100%) | 0  
chronology | 0 (0%) | 2  
circulationNotes | 0 (0%) | 2  
copyNumber | 0 (0%) | 2  
descriptionOfPieces | 0 (0%) | 2  
discoverySuppress | 0 (0%) | 2  
effectiveCallNumberComponents | 0 (0%) | 2  
effectiveLocationId | 0 (0%) | 2  
effectiveShelvingOrder | 0 (0%) | 2  
electronicAccess | 0 (0%) | 2  
enumeration | 0 (0%) | 2  
holdingsRecord2 | 0 (0%) | 2  
holdingsRecordId | 2 (100%) | 0  
hrid | 2 (100%) | 0  
id | 2 (100%) | 0  
inTransitDestinationServicePointId | 0 (0%) | 2  
itemDamagedStatusDate | 0 (0%) | 2  
itemDamagedStatusId | 0 (0%) | 2  
itemIdentifier | 0 (0%) | 2  
itemLevelCallNumber | 0 (0%) | 2  
itemLevelCallNumberPrefix | 0 (0%) | 2  
itemLevelCallNumberSuffix | 0 (0%) | 2  
itemLevelCallNumberTypeId | 0 (0%) | 2  
lastCheckIn | 0 (0%) | 2  
materialType | 0 (0%) | 2  
materialTypeId | 2 (100%) | 0  
metadata.createdByUserId | 2 (100%) | 0  
metadata.createdDate | 2 (100%) | 0  
metadata.updatedByUserId | 2 (100%) | 0  
metadata.updatedDate | 2 (100%) | 0  
missingPieces | 0 (0%) | 2  
missingPiecesDate | 0 (0%) | 2  
notes | 0 (0%) | 2  
numberOfMissingPieces | 0 (0%) | 2  
numberOfPieces | 0 (0%) | 2  
permanentLoanTypeId | 2 (100%) | 0  
permanentLocation | 0 (0%) | 2  
permanentLocationId | 0 (0%) | 2  
purchaseOrderLineIdentifier | 0 (0%) | 2  
statisticalCodeIds | 0 (0%) | 2  
status.date | 2 (100%) | 0  
status.name | 2 (100%) | 0  
tags | 0 (0%) | 2  
temporaryLoanTypeId | 0 (0%) | 2  
temporaryLocation | 0 (0%) | 2  
temporaryLocationId | 0 (0%) | 2  
volume | 0 (0%) | 2  
yearCaption | 0 (0%) | 2  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
Z30_BARCODE | 2 (100.0%) | 2 (100%) | 0  
Z30_MATERIAL | 4 (200.0%) | 4 (200%) | 0  
Z30_REC_KEY | 2 (100.0%) | 2 (100%) | 0  
fake_instance_id | 6 (300.0%) | 6 (300%) | 0  
</details>   
