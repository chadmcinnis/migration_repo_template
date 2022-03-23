# Bibliographic records transformation results   
Time Run: 2022-03-02T19:14:27.483089   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
   
## General statistics    
A list of general counterts to outline the transformation as a whole.    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
Lines written to identifier map | 12   
Records in file before parsing | 12   
Records successfully parsed from MARC21 | 12   
Records successfully transformed into FOLIO objects | 12   
Total number of Tags processed | 403   
</details>   
   
## Record status (leader pos 5)    
Library action: **Consider fixing d-values before migration**<br/>An overview of the Record statuses (Leader position 5) present in your source data.    Pay attention to the number of occurrences of the value 'd'. These d's are expressing that they are deleted, and the records might not work as expected in FOLIO. Consider marking them as suppressed in your current system and export them as a separate batch in order to have them suppressed in FOLIO. Allowed values according to the MARC standard are a,c,d,n,p    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
c | 2   
n | 10   
</details>   
   
## HRID Handling    
There are two ways of handling HRIDs. The default behaviour is to take the current 001 and move that to a new 035. This will also emerge as an Identifier on the Inventory Instances. The 001 and Instance HRID will be generated from the HRID settings in FOLIO. The second option is to maintain the 001s in the records, and also add this as the Instance HRID    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Added 035 from 001 | 12   
Created HRID using default settings | 12   
Values in 003: SE-LIBR | 2   
Values in 003: SwePub | 10   
</details>   
   
## Mapped identifier types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Identifier type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
020 -> ISBN | 2   
024 -> ISMN | 19   
024 -> Other Standard Identifier | 19   
024 -> UPC | 19   
035 -> System Control Number | 13   
</details>   
   
## Incomplete entity mapping adding entity    
**NO ACTION REQUIRED** <br/>This is a coding anomaly that FSE will look into.  <br/>Usually, the library does not have to do anything about it.<br/> One thing to look at is if there are many repeated subfields or unexpected patterns of subfields in the table.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
020 a:has_value ->>-->> identifiers identifierTypeId:'False' - value:'False'   | 2   
</details>   
   
## Mapped classification types    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Dewey | 1   
</details>   
   
## Mapped contributor name types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Name type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
100 -> Personal name | 12   
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
520 (Summary) -> Summary | 9   
546 (Language note) -> Language note | 1   
</details>   
   
## Matched Modes of issuance code    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Mode of issuace values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
single unit -- 9d18a02f-5897-4c31-9106-c9abb5c7ae8b | 12   
</details>   
   
## Language codes in records    
A breakdown of language codes occuring in the records. Purely informational.    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
eng | 12   
swe | 1   
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
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
264 ind2 1->Publication | 10   
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
Contributor type code Author found for $4 "aut" (aut)) | 52   
Contributor type code Originator found for $4 "org" (org)) | 10   
</details>   
   
## Instance format ids handling (337 + 338))    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
338$b is missing. Will try parse from 337$a and 338$b | 10   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 12  
administrativeNotes | 0 (0%) | 12  
alternativeTitles | 0 (0%) | 12  
catalogedDate | 0 (0%) | 12  
classifications | 0 (0%) | 12  
classifications.classificationNumber | 1 (8%) | 11  
classifications.classificationTypeId | 1 (8%) | 11  
contributors.contributorNameTypeId | 64 (533%) | 0  
contributors.contributorTypeId | 64 (533%) | 0  
contributors.contributorTypeText | 64 (533%) | 0  
contributors.name | 64 (533%) | 0  
contributors.primary | 12 (100%) | 0  
editions | 0 (0%) | 12  
electronicAccess | 0 (0%) | 12  
electronicAccess.linkText | 11 (92%) | 1  
electronicAccess.relationshipId | 21 (175%) | 0  
electronicAccess.uri | 21 (175%) | 0  
holdingsRecords2 | 0 (0%) | 12  
hrid | 12 (100%) | 0  
id | 12 (100%) | 0  
identifiers.identifierTypeId | 72 (600%) | 0  
identifiers.value | 72 (600%) | 0  
indexTitle | 12 (100%) | 0  
instanceFormats | 0 (0%) | 12  
instanceTypeId | 12 (100%) | 0  
matchKey | 0 (0%) | 12  
metadata.createdByUserId | 12 (100%) | 0  
metadata.createdDate | 12 (100%) | 0  
metadata.updatedByUserId | 12 (100%) | 0  
metadata.updatedDate | 12 (100%) | 0  
modeOfIssuanceId | 12 (100%) | 0  
natureOfContentTermIds | 0 (0%) | 12  
notes.instanceNoteTypeId | 23 (192%) | 0  
notes.note | 23 (192%) | 0  
physicalDescriptions | 0 (0%) | 12  
previouslyHeld | 0 (0%) | 12  
publication | 0 (0%) | 12  
publication.dateOfPublication | 11 (92%) | 1  
publication.place | 2 (17%) | 10  
publication.publisher | 7 (58%) | 5  
publication.role | 10 (83%) | 2  
publicationFrequency | 0 (0%) | 12  
publicationPeriod | 0 (0%) | 12  
publicationRange | 0 (0%) | 12  
series | 0 (0%) | 12  
source | 12 (100%) | 0  
sourceRecordFormat | 0 (0%) | 12  
statisticalCodeIds | 0 (0%) | 12  
statusId | 0 (0%) | 12  
statusUpdatedDate | 0 (0%) | 12  
subjects | 0 (0%) | 12  
tags | 0 (0%) | 12  
title | 12 (100%) | 0  
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
001 | 12 (100.0%) | 12 (100%) | 0  
003 | 12 (100.0%) | 0 (0%) | 12  
005 | 2 (16.7%) | 0 (0%) | 2  
008 | 12 (100.0%) | 12 (100%) | 0  
020 | 2 (16.7%) | 2 (17%) | 0  
024 | 19 (158.3%) | 19 (158%) | 0  
035 | 14 (116.7%) | 14 (117%) | 0  
040 | 12 (100.0%) | 0 (0%) | 12  
041 | 12 (100.0%) | 12 (100%) | 0  
042 | 12 (100.0%) | 0 (0%) | 12  
072 | 20 (166.7%) | 0 (0%) | 20  
082 | 1 (8.3%) | 1 (8%) | 0  
084 | 4 (33.3%) | 0 (0%) | 4  
100 | 12 (100.0%) | 12 (100%) | 0  
245 | 12 (100.0%) | 12 (100%) | 0  
260 | 1 (8.3%) | 1 (8%) | 0  
264 | 10 (83.3%) | 10 (83%) | 0  
300 | 2 (16.7%) | 2 (17%) | 0  
338 | 10 (83.3%) | 10 (83%) | 0  
440 | 2 (16.7%) | 0 (0%) | 2  
490 | 1 (8.3%) | 0 (0%) | 1  
500 | 12 (100.0%) | 12 (100%) | 0  
502 | 1 (8.3%) | 1 (8%) | 0  
520 | 9 (75.0%) | 9 (75%) | 0  
546 | 1 (8.3%) | 1 (8%) | 0  
599 | 1 (8.3%) | 0 (0%) | 1  
650 | 30 (250.0%) | 30 (250%) | 0  
653 | 53 (441.7%) | 0 (0%) | 53  
700 | 42 (350.0%) | 42 (350%) | 0  
710 | 10 (83.3%) | 10 (83%) | 0  
773 | 9 (75.0%) | 0 (0%) | 9  
830 | 1 (8.3%) | 1 (8%) | 0  
841 | 11 (91.7%) | 0 (0%) | 11  
852 | 12 (100.0%) | 0 (0%) | 12  
856 | 21 (175.0%) | 21 (175%) | 0  
887 | 4 (33.3%) | 0 (0%) | 4  
900 | 1 (8.3%) | 0 (0%) | 1  
976 | 1 (8.3%) | 0 (0%) | 1  
</details>   
