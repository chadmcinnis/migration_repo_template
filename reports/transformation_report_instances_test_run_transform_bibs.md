# Bibliographic records transformation results   
Time Run: 2022-03-02T19:14:27.483089   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
Lines written to identifier map | 14   
Records in file before parsing | 14   
Records successfully parsed from MARC21 | 14   
Records successfully transformed into FOLIO objects | 14   
Total number of Tags processed | 449   
</details>   
   
## Record status (leader pos 5)    
Library action: **Consider fixing d-values before migration**<br/>An overview of the Record statuses (Leader position 5) present in your source data.    Pay attention to the number of occurrences of the value 'd'. These d's are expressing that they are deleted, and the records might not work as expected in FOLIO. Consider marking them as suppressed in your current system and export them as a separate batch in order to have them suppressed in FOLIO. Allowed values according to the MARC standard are a,c,d,n,p    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
c | 4   
n | 10   
</details>   
   
## HRID Handling    
There are two ways of handling HRIDs. The default behaviour is to take the current 001 and move that to a new 035. This will also emerge as an Identifier on the Inventory Instances. The 001 and Instance HRID will be generated from the HRID settings in FOLIO. The second option is to maintain the 001s in the records, and also add this as the Instance HRID    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Added 035 from 001 | 14   
Created HRID using default settings | 14   
Values in 003: SE-LIBR | 4   
Values in 003: SwePub | 10   
</details>   
   
## Mapped identifier types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Identifier type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
020 -> ISBN | 3   
024 -> ISMN | 19   
024 -> Other Standard Identifier | 19   
024 -> UPC | 19   
035 -> System Control Number | 16   
</details>   
   
## Incomplete entity mapping adding entity    
**NO ACTION REQUIRED** <br/>This is a coding anomaly that FSE will look into.  <br/>Usually, the library does not have to do anything about it.<br/> One thing to look at is if there are many repeated subfields or unexpected patterns of subfields in the table.    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
020 a:has_value - q:has_value ->>-->> identifiers identifierTypeId:'False' - value:'True'   | 1   
020 a:has_value ->>-->> identifiers identifierTypeId:'False' - value:'False'   | 2   
</details>   
   
## Mapped classification types    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Dewey | 2   
</details>   
   
## Mapped contributor name types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Name type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
100 -> Personal name | 14   
700 -> Personal name | 42   
710 -> Corporate name | 10   
</details>   
   
## Mapped note types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Note type values.  <br/>The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
500 (General note) -> General note | 12   
502 (Dissertation note) -> Dissertation note | 1   
520 (Summary) -> Summary | 10   
546 (Language note) -> Language note | 1   
</details>   
   
## Matched Modes of issuance code    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Mode of issuace values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
single unit -- 9d18a02f-5897-4c31-9106-c9abb5c7ae8b | 14   
</details>   
   
## Language codes in records    
A breakdown of language codes occuring in the records. Purely informational.    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
eng | 12   
swe | 3   
</details>   
   
## Holdings generation from bibs    
Some libraries have Holdings/MFHD information baked into their bib records. The following breakdown gives an idea on the occurrence of 852/866 combinations    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Records with both 852s and at least one 86X | 2   
</details>   
   
## Mapped publisher role from Indicator2    
Publication Role, taken from the code in Ind2    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
264 ind2 1->Publication | 12   
264 ind2 3->Manufacture | 2   
</details>   
   
## Mapped electronic access relationships types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Electronic access relationship type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
No information provided | 20   
Related resource | 1   
</details>   
   
## Contributor type mapping    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Contributor type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
Contributor type code Author found for $4 "aut" (aut)) | 54   
Contributor type code Originator found for $4 "org" (org)) | 10   
</details>   
   
## Instance format ids handling (337 + 338))    
    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
338$b is missing. Will try parse from 337$a and 338$b | 10   
Successful match  - "nc"->unmediated -- volume | 1   
Successful match  - nc->unmediated -- volume | 1   
</details>   
   
## Resource Type Mapping (336)    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Instance type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
336$b text mapped from txt | 1   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 14  
administrativeNotes | 0 (0%) | 14  
alternativeTitles | 0 (0%) | 14  
catalogedDate | 0 (0%) | 14  
classifications | 0 (0%) | 14  
classifications.classificationNumber | 2 (14%) | 12  
classifications.classificationTypeId | 2 (14%) | 12  
contributors.contributorNameTypeId | 66 (471%) | 0  
contributors.contributorTypeId | 66 (471%) | 0  
contributors.contributorTypeText | 66 (471%) | 0  
contributors.name | 66 (471%) | 0  
contributors.primary | 14 (100%) | 0  
editions | 0 (0%) | 14  
electronicAccess | 0 (0%) | 14  
electronicAccess.linkText | 11 (79%) | 3  
electronicAccess.relationshipId | 21 (150%) | 0  
electronicAccess.uri | 21 (150%) | 0  
holdingsRecords2 | 0 (0%) | 14  
hrid | 14 (100%) | 0  
id | 14 (100%) | 0  
identifiers.identifierTypeId | 76 (543%) | 0  
identifiers.value | 76 (543%) | 0  
indexTitle | 14 (100%) | 0  
instanceFormats | 0 (0%) | 14  
instanceTypeId | 14 (100%) | 0  
matchKey | 0 (0%) | 14  
metadata.createdByUserId | 14 (100%) | 0  
metadata.createdDate | 14 (100%) | 0  
metadata.updatedByUserId | 14 (100%) | 0  
metadata.updatedDate | 14 (100%) | 0  
modeOfIssuanceId | 14 (100%) | 0  
natureOfContentTermIds | 0 (0%) | 14  
notes | 0 (0%) | 14  
notes.instanceNoteTypeId | 24 (171%) | 0  
notes.note | 24 (171%) | 0  
physicalDescriptions | 0 (0%) | 14  
previouslyHeld | 0 (0%) | 14  
publication | 0 (0%) | 14  
publication.dateOfPublication | 14 (100%) | 0  
publication.place | 5 (36%) | 9  
publication.publisher | 10 (71%) | 4  
publication.role | 14 (100%) | 0  
publicationFrequency | 0 (0%) | 14  
publicationPeriod | 0 (0%) | 14  
publicationRange | 0 (0%) | 14  
series | 0 (0%) | 14  
source | 14 (100%) | 0  
sourceRecordFormat | 0 (0%) | 14  
statisticalCodeIds | 0 (0%) | 14  
statusId | 0 (0%) | 14  
statusUpdatedDate | 0 (0%) | 14  
subjects | 0 (0%) | 14  
tags | 0 (0%) | 14  
title | 14 (100%) | 0  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
001 | 14 (100.0%) | 14 (100%) | 0  
003 | 14 (100.0%) | 0 (0%) | 14  
005 | 4 (28.6%) | 0 (0%) | 4  
008 | 14 (100.0%) | 14 (100%) | 0  
020 | 3 (21.4%) | 3 (21%) | 0  
024 | 19 (135.7%) | 19 (136%) | 0  
035 | 18 (128.6%) | 18 (129%) | 0  
040 | 14 (100.0%) | 0 (0%) | 14  
041 | 14 (100.0%) | 14 (100%) | 0  
042 | 12 (85.7%) | 0 (0%) | 12  
072 | 20 (142.9%) | 0 (0%) | 20  
082 | 2 (14.3%) | 2 (14%) | 0  
084 | 6 (42.9%) | 0 (0%) | 6  
100 | 14 (100.0%) | 14 (100%) | 0  
245 | 14 (100.0%) | 14 (100%) | 0  
260 | 1 (7.1%) | 1 (7%) | 0  
264 | 14 (100.0%) | 14 (100%) | 0  
300 | 4 (28.6%) | 4 (29%) | 0  
336 | 1 (7.1%) | 1 (7%) | 0  
337 | 1 (7.1%) | 0 (0%) | 1  
338 | 11 (78.6%) | 11 (79%) | 0  
440 | 2 (14.3%) | 0 (0%) | 2  
490 | 1 (7.1%) | 0 (0%) | 1  
500 | 12 (85.7%) | 12 (86%) | 0  
502 | 1 (7.1%) | 1 (7%) | 0  
520 | 10 (71.4%) | 10 (71%) | 0  
546 | 1 (7.1%) | 1 (7%) | 0  
599 | 1 (7.1%) | 0 (0%) | 1  
650 | 31 (221.4%) | 31 (221%) | 0  
653 | 53 (378.6%) | 0 (0%) | 53  
655 | 1 (7.1%) | 1 (7%) | 0  
700 | 42 (300.0%) | 42 (300%) | 0  
710 | 10 (71.4%) | 10 (71%) | 0  
773 | 9 (64.3%) | 0 (0%) | 9  
830 | 1 (7.1%) | 1 (7%) | 0  
841 | 11 (78.6%) | 0 (0%) | 11  
852 | 12 (85.7%) | 0 (0%) | 12  
856 | 21 (150.0%) | 21 (150%) | 0  
887 | 6 (42.9%) | 0 (0%) | 6  
900 | 1 (7.1%) | 0 (0%) | 1  
955 | 8 (57.1%) | 0 (0%) | 8  
976 | 1 (7.1%) | 0 (0%) | 1  
</details>   
