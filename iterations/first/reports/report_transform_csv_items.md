# Item transformation report   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
## Timings   
   
Measure | Value   
--- | ---:   
Time Started: | 2023-12-20T12:05:19.232314+00:00   
Time Finished: | 2023-12-20T12:33:56.531794+00:00   
Elapsed time: | 0:28:37.299480   
   
## General statistics    
A list of general counters to outline the transformation as a whole.    
<details><summary>Click to expand all 8 things</summary>     
   
Measure | Count   
--- | ---:   
Duplicate barcodes | 20   
Number of Legacy items in file_name='nalis_items.tsv' discovery_suppressed=False staff_suppressed=False service_point_id='' | 1,180,521   
Number of empty rows in nalis_items.tsv | 0   
Number of files processed | 1   
Number of legacy items in total | 1,180,521   
Number of records written to disk | 1,180,521   
Number of rows in nalis_items.tsv | 1,180,521   
</details>   
   
## Callnumber type mapping    
Call number types in MFHDs are mapped from 852, Indicator 1 according to a certain scheme. (LOC documentation)[https://www.loc.gov/marc/holdings/hd852.html]    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
Unmapped (Default value was set) -- 03dd64d00-5626-4ecd-8ece-4531e0069f35 -> Other scheme | 1,151,933   
Unmapped (Default value was set) -- 95467209-6d7b-468b-94df-0f5d7ad2747d -> Other scheme | 28,588   
</details>   
   
## FOLIO default values added    
The below FOLIO default values were added to records that had no mapped value in the source data.    
<details><summary>Click to expand all 9 things</summary>     
   
Measure | Count   
--- | ---:   
 added to descriptionOfPieces | 1,178,700   
 added to notes[0].note | 1,074,421   
 added to notes[2].note | 16,828   
 added to notes[3].note | 57,696   
 added to notes[4].note | 15,971   
 added to notes[5].note | 1,170,751   
 added to numberOfPieces | 1,178,700   
 added to volume | 1,180,521   
</details>   
   
## Unmapped properties    
    
<details><summary>Click to expand all 15 things</summary>     
   
Measure | Count   
--- | ---:   
descriptionOfPieces | 1,178,700   
notes[0].note | 1,074,421   
notes[0].staffOnly | 1,180,521   
notes[1].staffOnly | 1,180,521   
notes[2].note | 16,828   
notes[2].staffOnly | 1,180,521   
notes[3].note | 57,696   
notes[3].staffOnly | 1,180,521   
notes[4].note | 15,971   
notes[4].staffOnly | 1,180,521   
notes[5].note | 1,170,751   
notes[5].staffOnly | 1,180,521   
numberOfPieces | 1,178,700   
volume | 1,180,521   
</details>   
   
## Default values from mapping added    
The values below were added to all records from the 'value' field in the mapping file, overriding any mapped values from the source data.    
<details><summary>Click to expand all 13 things</summary>     
   
Measure | Count   
--- | ---:   
1fbeaf4e-0ecb-47bd-83bf-a717bd390527 added to notes[4].itemNoteTypeId | 1,180,521   
26c03dca-da5e-401b-bd54-290bec7cd267 added to notes[5].itemNoteTypeId | 1,180,521   
4f13c23a-e2bb-4cc2-99ea-6b018a929323 added to notes[3].itemNoteTypeId | 1,180,521   
781a9208-ed61-4c2e-9b2c-2bbfed2ce488 added to notes[0].itemNoteTypeId | 1,180,521   
82019387-3cda-464f-88e5-d040a87ef5c3 added to notes[2].itemNoteTypeId | 1,180,521   
976ba776-d9c9-414c-85a4-dcf6afa8563d added to notes[1].itemNoteTypeId | 1,180,521   
False added to notes[0].staffOnly | 1,180,521   
False added to notes[1].staffOnly | 1,180,521   
False added to notes[2].staffOnly | 1,180,521   
False added to notes[3].staffOnly | 1,180,521   
False added to notes[4].staffOnly | 1,180,521   
False added to notes[5].staffOnly | 1,180,521   
</details>   
   
## Status mapping    
    
<details><summary>Click to expand all 15 things</summary>     
   
Measure | Count   
--- | ---:   
'AVAIL_SOON' -> Available | 984   
'Available' -> Available | 294,510   
'BINDERY' -> In process | 4,712   
'CATALOGING' -> In process | 93,758   
'CHECKEDOUT' -> Available | 239,204   
'DISCARD' -> Withdrawn | 51,756   
'HOLDS' -> Available | 461   
'INTRANSIT' -> Available | 249,572   
'LOST-ASSUM' -> Missing | 89   
'LOST-CLAIM' -> Missing | 9,154   
'LOST-PAID' -> Available | 1,598   
'MISSING' -> Available | 4,176   
'STORAGE' -> Unavailable | 230,505   
'WITHDRAWN' -> Withdrawn | 42   
</details>   
   
## Mapped Material Types    
    
<details><summary>Click to expand all 48 things</summary>     
   
Measure | Count   
--- | ---:   
AUDIO -> Sound recording | 36,616   
BOOK -> Book | 411,217   
COMP-FILE -> CD | 987   
EBOOK -> Electronic resource | 5   
GRAPHIC -> Graphic Novel | 4   
JVIDEO -> Video recording (inclusive of DVD) | 13,154   
KIT -> Visual materials (VM) | 239   
MAGAZINE -> CNR | 244   
MAP -> Map | 30   
MIXED -> Mixed | 1   
MUSIC -> Music | 367   
NEWSPAPER -> CNR | 4   
Unmapped (Default value was set) -- ARTIFACT -> Book | 3   
Unmapped (Default value was set) -- BRL -> Book | 4   
Unmapped (Default value was set) -- ILL-BOOK -> Book | 1   
Unmapped (Default value was set) -- JAUDIO -> Book | 5,069   
Unmapped (Default value was set) -- JBOOK -> Book | 365,851   
Unmapped (Default value was set) -- JCOMP-FILE -> Book | 654   
Unmapped (Default value was set) -- JMUSIC -> Book | 137   
Unmapped (Default value was set) -- JREF-AUDIO -> Book | 550   
Unmapped (Default value was set) -- JREF-BOOK -> Book | 10,357   
Unmapped (Default value was set) -- JREF-MUSIC -> Book | 61   
Unmapped (Default value was set) -- JREF-VIDEO -> Book | 1,141   
Unmapped (Default value was set) -- JREFCO-FIL -> Book | 94   
Unmapped (Default value was set) -- LAPTOP -> Book | 14   
Unmapped (Default value was set) -- LIB-COLL -> Book | 2,594   
Unmapped (Default value was set) -- MUSIC_PRN -> Book | 12   
Unmapped (Default value was set) -- NEW-BOOK -> Book | 1   
Unmapped (Default value was set) -- PAMPHLET -> Book | 79   
Unmapped (Default value was set) -- PTC -> Book | 996   
Unmapped (Default value was set) -- PTL -> Book | 1,529   
Unmapped (Default value was set) -- REF-AUDIO -> Book | 4,099   
Unmapped (Default value was set) -- REF-BOOK -> Book | 113,036   
Unmapped (Default value was set) -- REF-MUSIC -> Book | 1,122   
Unmapped (Default value was set) -- REF-VIDEO -> Book | 2,324   
Unmapped (Default value was set) -- REFCO-FILE -> Book | 693   
Unmapped (Default value was set) -- UNKNOWN -> Book | 21,583   
Unmapped (Default value was set) -- VIDEO -> Book | 21,811   
Unmapped (Default value was set) -- YAAUDIO -> Book | 5,577   
Unmapped (Default value was set) -- YABOOK -> Book | 134,143   
Unmapped (Default value was set) -- YAMUSIC -> Book | 3   
Unmapped (Default value was set) -- YAREF-AUD -> Book | 127   
Unmapped (Default value was set) -- YAREF-BOOK -> Book | 11,432   
Unmapped (Default value was set) -- YAREF-VID -> Book | 223   
Unmapped (Default value was set) -- YAREFCO-FI -> Book | 586   
Unmapped (Default value was set) -- YAVIDEO -> Book | 10,490   
Unmapped (Default value was set) -- YCOMP-FILE -> Book | 1,257   
</details>   
   
## Permanent Loan type mapping    
    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
Unmapped (Default value was set) -- M -> Can circulate | 258,776   
Unmapped (Default value was set) -- N -> Can circulate | 95,050   
Unmapped (Default value was set) -- Y -> Can circulate | 826,695   
</details>   
   
## Location mapping    
These are the results for the mapping between legacy locations and your new FOLIO location structure    
<details><summary>Click to expand all 639 things</summary>     
   
Measure | Count   
--- | ---:   
Unmapped (Default value was set) -- ARIAFI -> MIGRATION | 1   
Unmapped (Default value was set) -- ARIBINDERY -> MIGRATION | 7   
Unmapped (Default value was set) -- ARICATALOGING -> MIGRATION | 1   
Unmapped (Default value was set) -- ARIEAS -> MIGRATION | 1,451   
Unmapped (Default value was set) -- ARIJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- ARIJNF -> MIGRATION | 2   
Unmapped (Default value was set) -- ARILIB -> MIGRATION | 1   
Unmapped (Default value was set) -- ARILIBCOLL -> MIGRATION | 108   
Unmapped (Default value was set) -- ARIMEDIACTR -> MIGRATION | 3,575   
Unmapped (Default value was set) -- ARIMMC -> MIGRATION | 12   
Unmapped (Default value was set) -- ARIPERRACK -> MIGRATION | 7   
Unmapped (Default value was set) -- ARIPTC -> MIGRATION | 6   
Unmapped (Default value was set) -- ARIPTL -> MIGRATION | 137   
Unmapped (Default value was set) -- ARIREFERENCE -> MIGRATION | 140   
Unmapped (Default value was set) -- ARISPINNERS -> MIGRATION | 3,776   
Unmapped (Default value was set) -- ARISTACKS -> MIGRATION | 39,383   
Unmapped (Default value was set) -- ARISTE -> MIGRATION | 8   
Unmapped (Default value was set) -- ARIUNKNOWN -> MIGRATION | 2   
Unmapped (Default value was set) -- ARUSTACKS -> MIGRATION | 1   
Unmapped (Default value was set) -- BARCATALOGING -> MIGRATION | 1   
Unmapped (Default value was set) -- BAREAS -> MIGRATION | 162   
Unmapped (Default value was set) -- BARMEDIACTR -> MIGRATION | 434   
Unmapped (Default value was set) -- BARPTL -> MIGRATION | 11   
Unmapped (Default value was set) -- BARREFERENCE -> MIGRATION | 13   
Unmapped (Default value was set) -- BARSPINNERS -> MIGRATION | 488   
Unmapped (Default value was set) -- BARSTACKS -> MIGRATION | 3,140   
Unmapped (Default value was set) -- BARUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- BETANR -> MIGRATION | 2   
Unmapped (Default value was set) -- BETCATALOGING -> MIGRATION | 1   
Unmapped (Default value was set) -- BETEAS -> MIGRATION | 71   
Unmapped (Default value was set) -- BETMEDIACTR -> MIGRATION | 115   
Unmapped (Default value was set) -- BETPTL -> MIGRATION | 5   
Unmapped (Default value was set) -- BETREFERENCE -> MIGRATION | 25   
Unmapped (Default value was set) -- BETSPINNERS -> MIGRATION | 400   
Unmapped (Default value was set) -- BETSTACKS -> MIGRATION | 1,411   
Unmapped (Default value was set) -- BM0EAS -> MIGRATION | 1,095   
Unmapped (Default value was set) -- BM0MEDIACTR -> MIGRATION | 1,057   
Unmapped (Default value was set) -- BM0PTL -> MIGRATION | 12   
Unmapped (Default value was set) -- BM0REFERENCE -> MIGRATION | 36   
Unmapped (Default value was set) -- BM0SPINNERS -> MIGRATION | 963   
Unmapped (Default value was set) -- BM0STACKS -> MIGRATION | 13,606   
Unmapped (Default value was set) -- BM0UNKNOWN -> MIGRATION | 2   
Unmapped (Default value was set) -- BM1EAS -> MIGRATION | 1,174   
Unmapped (Default value was set) -- BM1JNF -> MIGRATION | 2   
Unmapped (Default value was set) -- BM1MEDIACTR -> MIGRATION | 235   
Unmapped (Default value was set) -- BM1PERRACK -> MIGRATION | 2   
Unmapped (Default value was set) -- BM1PTL -> MIGRATION | 10   
Unmapped (Default value was set) -- BM1REFERENCE -> MIGRATION | 22   
Unmapped (Default value was set) -- BM1SPINNERS -> MIGRATION | 1,416   
Unmapped (Default value was set) -- BM1STACKS -> MIGRATION | 14,666   
Unmapped (Default value was set) -- BM2AFI -> MIGRATION | 35   
Unmapped (Default value was set) -- BM2ANF -> MIGRATION | 6   
Unmapped (Default value was set) -- BM2DISCARD -> MIGRATION | 1   
Unmapped (Default value was set) -- BM2EAS -> MIGRATION | 434   
Unmapped (Default value was set) -- BM2JFI -> MIGRATION | 40   
Unmapped (Default value was set) -- BM2JNF -> MIGRATION | 38   
Unmapped (Default value was set) -- BM2LIBCOLL -> MIGRATION | 1   
Unmapped (Default value was set) -- BM2MEDIACTR -> MIGRATION | 146   
Unmapped (Default value was set) -- BM2PERRACK -> MIGRATION | 2   
Unmapped (Default value was set) -- BM2PTL -> MIGRATION | 7   
Unmapped (Default value was set) -- BM2REFERENCE -> MIGRATION | 3   
Unmapped (Default value was set) -- BM2REPAIR -> MIGRATION | 1   
Unmapped (Default value was set) -- BM2SPINNERS -> MIGRATION | 1,103   
Unmapped (Default value was set) -- BM2STACKS -> MIGRATION | 5,953   
Unmapped (Default value was set) -- BM2YFI -> MIGRATION | 87   
Unmapped (Default value was set) -- BM2YNF -> MIGRATION | 6   
Unmapped (Default value was set) -- BM3DOW -> MIGRATION | 1   
Unmapped (Default value was set) -- BM3EAS -> MIGRATION | 996   
Unmapped (Default value was set) -- BM3JNF -> MIGRATION | 2   
Unmapped (Default value was set) -- BM3MEDIACTR -> MIGRATION | 854   
Unmapped (Default value was set) -- BM3PERRACK -> MIGRATION | 2   
Unmapped (Default value was set) -- BM3PTL -> MIGRATION | 28   
Unmapped (Default value was set) -- BM3REFERENCE -> MIGRATION | 19   
Unmapped (Default value was set) -- BM3SMA -> MIGRATION | 1   
Unmapped (Default value was set) -- BM3SPINNERS -> MIGRATION | 2,096   
Unmapped (Default value was set) -- BM3STACKS -> MIGRATION | 15,101   
Unmapped (Default value was set) -- BM3STORAGE -> MIGRATION | 1   
Unmapped (Default value was set) -- BM4BINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- BM4EAS -> MIGRATION | 346   
Unmapped (Default value was set) -- BM4JNF -> MIGRATION | 2   
Unmapped (Default value was set) -- BM4MEDIACTR -> MIGRATION | 199   
Unmapped (Default value was set) -- BM4PERRACK -> MIGRATION | 2   
Unmapped (Default value was set) -- BM4PTL -> MIGRATION | 31   
Unmapped (Default value was set) -- BM4REFERENCE -> MIGRATION | 9   
Unmapped (Default value was set) -- BM4SPINNERS -> MIGRATION | 1,038   
Unmapped (Default value was set) -- BM4STACKS -> MIGRATION | 7,981   
Unmapped (Default value was set) -- CARAMC -> MIGRATION | 122   
Unmapped (Default value was set) -- CARBRL -> MIGRATION | 2   
Unmapped (Default value was set) -- CARCATALOGING -> MIGRATION | 2   
Unmapped (Default value was set) -- CARDISCARD -> MIGRATION | 1   
Unmapped (Default value was set) -- CAREAS -> MIGRATION | 1,885   
Unmapped (Default value was set) -- CARJMC -> MIGRATION | 2   
Unmapped (Default value was set) -- CARJNF -> MIGRATION | 3   
Unmapped (Default value was set) -- CARLIBCOLL -> MIGRATION | 286   
Unmapped (Default value was set) -- CARMEDIACTR -> MIGRATION | 4,246   
Unmapped (Default value was set) -- CARMMC -> MIGRATION | 45   
Unmapped (Default value was set) -- CARPERRACK -> MIGRATION | 17   
Unmapped (Default value was set) -- CARPTC -> MIGRATION | 24   
Unmapped (Default value was set) -- CARPTL -> MIGRATION | 218   
Unmapped (Default value was set) -- CARREFERENCE -> MIGRATION | 271   
Unmapped (Default value was set) -- CARRESERVES -> MIGRATION | 1   
Unmapped (Default value was set) -- CARSMA -> MIGRATION | 3   
Unmapped (Default value was set) -- CARSPINNERS -> MIGRATION | 5,496   
Unmapped (Default value was set) -- CARST -> MIGRATION | 1   
Unmapped (Default value was set) -- CARSTACKS -> MIGRATION | 61,928   
Unmapped (Default value was set) -- CARSTC -> MIGRATION | 1   
Unmapped (Default value was set) -- CARSTORAGE -> MIGRATION | 1   
Unmapped (Default value was set) -- CARUNKNOWN -> MIGRATION | 23   
Unmapped (Default value was set) -- CARWITHDRAWN -> MIGRATION | 1   
Unmapped (Default value was set) -- CEDEAS -> MIGRATION | 453   
Unmapped (Default value was set) -- CEDJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- CEDMEDIACTR -> MIGRATION | 953   
Unmapped (Default value was set) -- CEDMISSING -> MIGRATION | 2   
Unmapped (Default value was set) -- CEDPERRACK -> MIGRATION | 3   
Unmapped (Default value was set) -- CEDPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- CEDPTL -> MIGRATION | 17   
Unmapped (Default value was set) -- CEDREFERENCE -> MIGRATION | 31   
Unmapped (Default value was set) -- CEDSPINNERS -> MIGRATION | 737   
Unmapped (Default value was set) -- CEDSTACKS -> MIGRATION | 9,529   
Unmapped (Default value was set) -- CHABINDERY -> MIGRATION | 4   
Unmapped (Default value was set) -- CHACATALOGING -> MIGRATION | 2   
Unmapped (Default value was set) -- CHAEAS -> MIGRATION | 977   
Unmapped (Default value was set) -- CHAJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- CHAJNF -> MIGRATION | 2   
Unmapped (Default value was set) -- CHALAC -> MIGRATION | 1   
Unmapped (Default value was set) -- CHALIB -> MIGRATION | 1   
Unmapped (Default value was set) -- CHALIBCOLL -> MIGRATION | 103   
Unmapped (Default value was set) -- CHAMEDIACTR -> MIGRATION | 3,900   
Unmapped (Default value was set) -- CHAMMC -> MIGRATION | 9   
Unmapped (Default value was set) -- CHAPERRACK -> MIGRATION | 5   
Unmapped (Default value was set) -- CHAPTC -> MIGRATION | 4   
Unmapped (Default value was set) -- CHAPTL -> MIGRATION | 88   
Unmapped (Default value was set) -- CHAREFERENCE -> MIGRATION | 220   
Unmapped (Default value was set) -- CHASMA -> MIGRATION | 1   
Unmapped (Default value was set) -- CHASPINNERS -> MIGRATION | 4,158   
Unmapped (Default value was set) -- CHASTACKS -> MIGRATION | 28,878   
Unmapped (Default value was set) -- CHLBINDERY -> MIGRATION | 26   
Unmapped (Default value was set) -- CHLDISCARD -> MIGRATION | 513   
Unmapped (Default value was set) -- CHLEAS -> MIGRATION | 565   
Unmapped (Default value was set) -- CHLMEDIACTR -> MIGRATION | 215   
Unmapped (Default value was set) -- CHLPTL -> MIGRATION | 1   
Unmapped (Default value was set) -- CHLREFERENCE -> MIGRATION | 47   
Unmapped (Default value was set) -- CHLREPAIR -> MIGRATION | 64   
Unmapped (Default value was set) -- CHLRES -> MIGRATION | 26   
Unmapped (Default value was set) -- CHLRESERVES -> MIGRATION | 89   
Unmapped (Default value was set) -- CHLSPINNERS -> MIGRATION | 5   
Unmapped (Default value was set) -- CHLSTACKS -> MIGRATION | 13,934   
Unmapped (Default value was set) -- CHLSTORAGE -> MIGRATION | 383   
Unmapped (Default value was set) -- CHLWITHDRAWN -> MIGRATION | 2,794   
Unmapped (Default value was set) -- CVABINDERY -> MIGRATION | 3   
Unmapped (Default value was set) -- CVACATALOGING -> MIGRATION | 5   
Unmapped (Default value was set) -- CVAEAS -> MIGRATION | 1,095   
Unmapped (Default value was set) -- CVAJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- CVAJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- CVALIBCOLL -> MIGRATION | 31   
Unmapped (Default value was set) -- CVALOST -> MIGRATION | 3   
Unmapped (Default value was set) -- CVAMEDIACTR -> MIGRATION | 2,114   
Unmapped (Default value was set) -- CVAMMC -> MIGRATION | 7   
Unmapped (Default value was set) -- CVAPERRACK -> MIGRATION | 5   
Unmapped (Default value was set) -- CVAPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- CVAPTL -> MIGRATION | 90   
Unmapped (Default value was set) -- CVAREFERENCE -> MIGRATION | 111   
Unmapped (Default value was set) -- CVASPINNERS -> MIGRATION | 2,470   
Unmapped (Default value was set) -- CVAST -> MIGRATION | 1   
Unmapped (Default value was set) -- CVASTACKS -> MIGRATION | 30,683   
Unmapped (Default value was set) -- CVAUNKNOWN -> MIGRATION | 35   
Unmapped (Default value was set) -- CVAYMC -> MIGRATION | 1   
Unmapped (Default value was set) -- DEBEAS -> MIGRATION | 597   
Unmapped (Default value was set) -- DEBJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- DEBJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- DEBMEDIACTR -> MIGRATION | 1,400   
Unmapped (Default value was set) -- DEBMMC -> MIGRATION | 4   
Unmapped (Default value was set) -- DEBPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- DEBPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- DEBPTL -> MIGRATION | 33   
Unmapped (Default value was set) -- DEBREFERENCE -> MIGRATION | 70   
Unmapped (Default value was set) -- DEBSPINNERS -> MIGRATION | 1,249   
Unmapped (Default value was set) -- DEBSTACKS -> MIGRATION | 16,066   
Unmapped (Default value was set) -- DEBUNKNOWN -> MIGRATION | 2   
Unmapped (Default value was set) -- DGMBINDERY -> MIGRATION | 3   
Unmapped (Default value was set) -- DGMCATALOGING -> MIGRATION | 1   
Unmapped (Default value was set) -- DGMDISCARD -> MIGRATION | 3   
Unmapped (Default value was set) -- DGMEAS -> MIGRATION | 210   
Unmapped (Default value was set) -- DGMJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- DGMJNF -> MIGRATION | 2   
Unmapped (Default value was set) -- DGMLIBCOLL -> MIGRATION | 4   
Unmapped (Default value was set) -- DGMMEDIACTR -> MIGRATION | 1,651   
Unmapped (Default value was set) -- DGMMMC -> MIGRATION | 5   
Unmapped (Default value was set) -- DGMPERRACK -> MIGRATION | 5   
Unmapped (Default value was set) -- DGMPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- DGMPTL -> MIGRATION | 62   
Unmapped (Default value was set) -- DGMREFERENCE -> MIGRATION | 73   
Unmapped (Default value was set) -- DGMSPINNERS -> MIGRATION | 2,148   
Unmapped (Default value was set) -- DGMSTACKS -> MIGRATION | 19,301   
Unmapped (Default value was set) -- DGMUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- DGMYFI -> MIGRATION | 1   
Unmapped (Default value was set) -- HERAW1 -> MIGRATION | 4   
Unmapped (Default value was set) -- HERBINDERY -> MIGRATION | 15   
Unmapped (Default value was set) -- HERCATALOGING -> MIGRATION | 34   
Unmapped (Default value was set) -- HEREAS -> MIGRATION | 1   
Unmapped (Default value was set) -- HEREIC -> MIGRATION | 50   
Unmapped (Default value was set) -- HERGOV -> MIGRATION | 25   
Unmapped (Default value was set) -- HERHERITAGE -> MIGRATION | 1,093   
Unmapped (Default value was set) -- HERHSC -> MIGRATION | 5   
Unmapped (Default value was set) -- HERINPROCESS -> MIGRATION | 44   
Unmapped (Default value was set) -- HERJMC -> MIGRATION | 2   
Unmapped (Default value was set) -- HERLED -> MIGRATION | 18   
Unmapped (Default value was set) -- HERLIBCOLL -> MIGRATION | 67   
Unmapped (Default value was set) -- HERMAP -> MIGRATION | 1   
Unmapped (Default value was set) -- HERMEDIACTR -> MIGRATION | 1,678   
Unmapped (Default value was set) -- HERMISSING -> MIGRATION | 1   
Unmapped (Default value was set) -- HERMMC -> MIGRATION | 114   
Unmapped (Default value was set) -- HERPERRACK -> MIGRATION | 104   
Unmapped (Default value was set) -- HERPTC -> MIGRATION | 6   
Unmapped (Default value was set) -- HERPTL -> MIGRATION | 1   
Unmapped (Default value was set) -- HERRBC -> MIGRATION | 13   
Unmapped (Default value was set) -- HERREFERENCE -> MIGRATION | 388   
Unmapped (Default value was set) -- HERRES -> MIGRATION | 1   
Unmapped (Default value was set) -- HERSPINNERS -> MIGRATION | 23   
Unmapped (Default value was set) -- HERST -> MIGRATION | 1   
Unmapped (Default value was set) -- HERSTACKS -> MIGRATION | 43,584   
Unmapped (Default value was set) -- HERSTC -> MIGRATION | 22   
Unmapped (Default value was set) -- HERSTE -> MIGRATION | 191   
Unmapped (Default value was set) -- HERUNKNOWN -> MIGRATION | 11   
Unmapped (Default value was set) -- LABBINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- LABEAS -> MIGRATION | 644   
Unmapped (Default value was set) -- LABJMC -> MIGRATION | 2   
Unmapped (Default value was set) -- LABJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- LABMAP -> MIGRATION | 1   
Unmapped (Default value was set) -- LABMEDIACTR -> MIGRATION | 1,645   
Unmapped (Default value was set) -- LABMMC -> MIGRATION | 7   
Unmapped (Default value was set) -- LABPERRACK -> MIGRATION | 3   
Unmapped (Default value was set) -- LABPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- LABPTL -> MIGRATION | 47   
Unmapped (Default value was set) -- LABREFERENCE -> MIGRATION | 46   
Unmapped (Default value was set) -- LABSPINNERS -> MIGRATION | 1,330   
Unmapped (Default value was set) -- LABSTACKS -> MIGRATION | 14,843   
Unmapped (Default value was set) -- LABUNKNOWN -> MIGRATION | 2   
Unmapped (Default value was set) -- MALBINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- MALBRL -> MIGRATION | 1   
Unmapped (Default value was set) -- MALEAS -> MIGRATION | 696   
Unmapped (Default value was set) -- MALJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- MALJNF -> MIGRATION | 2   
Unmapped (Default value was set) -- MALLIBCOLL -> MIGRATION | 18   
Unmapped (Default value was set) -- MALMEDIACTR -> MIGRATION | 2,532   
Unmapped (Default value was set) -- MALMMC -> MIGRATION | 9   
Unmapped (Default value was set) -- MALPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- MALPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- MALPTL -> MIGRATION | 63   
Unmapped (Default value was set) -- MALREFERENCE -> MIGRATION | 50   
Unmapped (Default value was set) -- MALSPINNERS -> MIGRATION | 1,676   
Unmapped (Default value was set) -- MALSTACKS -> MIGRATION | 18,327   
Unmapped (Default value was set) -- MALUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- MAYBINDERY -> MIGRATION | 4   
Unmapped (Default value was set) -- MAYEAS -> MIGRATION | 977   
Unmapped (Default value was set) -- MAYJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- MAYJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- MAYLIBCOLL -> MIGRATION | 10   
Unmapped (Default value was set) -- MAYMEDIACTR -> MIGRATION | 2,489   
Unmapped (Default value was set) -- MAYMMC -> MIGRATION | 7   
Unmapped (Default value was set) -- MAYPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- MAYPTC -> MIGRATION | 2   
Unmapped (Default value was set) -- MAYPTL -> MIGRATION | 81   
Unmapped (Default value was set) -- MAYREFERENCE -> MIGRATION | 120   
Unmapped (Default value was set) -- MAYSPINNERS -> MIGRATION | 3,672   
Unmapped (Default value was set) -- MAYSTACKS -> MIGRATION | 24,940   
Unmapped (Default value was set) -- MAYUNKNOWN -> MIGRATION | 6   
Unmapped (Default value was set) -- MGAANR -> MIGRATION | 1   
Unmapped (Default value was set) -- MGABINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- MGAEAS -> MIGRATION | 722   
Unmapped (Default value was set) -- MGAJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- MGAJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- MGALIBCOLL -> MIGRATION | 1   
Unmapped (Default value was set) -- MGAMEDIACTR -> MIGRATION | 1,808   
Unmapped (Default value was set) -- MGAMMC -> MIGRATION | 6   
Unmapped (Default value was set) -- MGAPERRACK -> MIGRATION | 3   
Unmapped (Default value was set) -- MGAPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- MGAPTL -> MIGRATION | 66   
Unmapped (Default value was set) -- MGAREFERENCE -> MIGRATION | 44   
Unmapped (Default value was set) -- MGASPINNERS -> MIGRATION | 1,304   
Unmapped (Default value was set) -- MGASTACKS -> MIGRATION | 13,951   
Unmapped (Default value was set) -- MHLEAS -> MIGRATION | 68   
Unmapped (Default value was set) -- MHLJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- MHLLIBCOLL -> MIGRATION | 7   
Unmapped (Default value was set) -- MHLMEDIACTR -> MIGRATION | 343   
Unmapped (Default value was set) -- MHLMMC -> MIGRATION | 2   
Unmapped (Default value was set) -- MHLPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- MHLPTL -> MIGRATION | 8   
Unmapped (Default value was set) -- MHLREFERENCE -> MIGRATION | 17   
Unmapped (Default value was set) -- MHLSPINNERS -> MIGRATION | 559   
Unmapped (Default value was set) -- MHLSTACKS -> MIGRATION | 2,510   
Unmapped (Default value was set) -- MHLTES -> MIGRATION | 1   
Unmapped (Default value was set) -- MHLUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- MSPMEDIACTR -> MIGRATION | 137   
Unmapped (Default value was set) -- MSPPERRACK -> MIGRATION | 3   
Unmapped (Default value was set) -- MSPPTL -> MIGRATION | 1   
Unmapped (Default value was set) -- MSPREFERENCE -> MIGRATION | 42   
Unmapped (Default value was set) -- MSPSPINNERS -> MIGRATION | 413   
Unmapped (Default value was set) -- MSPST -> MIGRATION | 1   
Unmapped (Default value was set) -- MSPSTACKS -> MIGRATION | 2,698   
Unmapped (Default value was set) -- PFOBRL -> MIGRATION | 1   
Unmapped (Default value was set) -- PFOEAS -> MIGRATION | 758   
Unmapped (Default value was set) -- PFOJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- PFOJNF -> MIGRATION | 2   
Unmapped (Default value was set) -- PFOLIBCOLL -> MIGRATION | 16   
Unmapped (Default value was set) -- PFOMEDIACTR -> MIGRATION | 2,692   
Unmapped (Default value was set) -- PFOMMC -> MIGRATION | 13   
Unmapped (Default value was set) -- PFOPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- PFOPTC -> MIGRATION | 2   
Unmapped (Default value was set) -- PFOPTL -> MIGRATION | 71   
Unmapped (Default value was set) -- PFOREFERENCE -> MIGRATION | 65   
Unmapped (Default value was set) -- PFOSPINNERS -> MIGRATION | 1,965   
Unmapped (Default value was set) -- PFOSTACKS -> MIGRATION | 22,340   
Unmapped (Default value was set) -- POSALAMC -> MIGRATION | 13   
Unmapped (Default value was set) -- POSALANF -> MIGRATION | 1   
Unmapped (Default value was set) -- POSALBINDERY -> MIGRATION | 31   
Unmapped (Default value was set) -- POSALCATALOGING -> MIGRATION | 12   
Unmapped (Default value was set) -- POSALDLS -> MIGRATION | 6   
Unmapped (Default value was set) -- POSALEAS -> MIGRATION | 2   
Unmapped (Default value was set) -- POSALHRM -> MIGRATION | 2   
Unmapped (Default value was set) -- POSALIFN -> MIGRATION | 127   
Unmapped (Default value was set) -- POSALINPROCESS -> MIGRATION | 5   
Unmapped (Default value was set) -- POSALINTRANSIT -> MIGRATION | 1   
Unmapped (Default value was set) -- POSALITC -> MIGRATION | 1   
Unmapped (Default value was set) -- POSALLIB -> MIGRATION | 1   
Unmapped (Default value was set) -- POSALLIBCOLL -> MIGRATION | 1,674   
Unmapped (Default value was set) -- POSALMEDIACTR -> MIGRATION | 4,478   
Unmapped (Default value was set) -- POSALMMC -> MIGRATION | 46   
Unmapped (Default value was set) -- POSALPBL -> MIGRATION | 31   
Unmapped (Default value was set) -- POSALPERRACK -> MIGRATION | 24   
Unmapped (Default value was set) -- POSALPTC -> MIGRATION | 318   
Unmapped (Default value was set) -- POSALPTL -> MIGRATION | 48   
Unmapped (Default value was set) -- POSALREFERENCE -> MIGRATION | 433   
Unmapped (Default value was set) -- POSALRESERVES -> MIGRATION | 598   
Unmapped (Default value was set) -- POSALSMA -> MIGRATION | 1   
Unmapped (Default value was set) -- POSALSPINNERS -> MIGRATION | 7,782   
Unmapped (Default value was set) -- POSALSTACKS -> MIGRATION | 120,677   
Unmapped (Default value was set) -- POSALSTE -> MIGRATION | 4   
Unmapped (Default value was set) -- POSALTRG -> MIGRATION | 7   
Unmapped (Default value was set) -- POSALUNKNOWN -> MIGRATION | 10   
Unmapped (Default value was set) -- POSALWITHDRAWN -> MIGRATION | 2   
Unmapped (Default value was set) -- POSCLBINDERY -> MIGRATION | 14   
Unmapped (Default value was set) -- POSCLBRL -> MIGRATION | 2   
Unmapped (Default value was set) -- POSCLEAS -> MIGRATION | 9,803   
Unmapped (Default value was set) -- POSCLJMC -> MIGRATION | 2   
Unmapped (Default value was set) -- POSCLJNF -> MIGRATION | 3   
Unmapped (Default value was set) -- POSCLLIBCOLL -> MIGRATION | 18   
Unmapped (Default value was set) -- POSCLMEDIACTR -> MIGRATION | 2,388   
Unmapped (Default value was set) -- POSCLMMC -> MIGRATION | 10   
Unmapped (Default value was set) -- POSCLPTC -> MIGRATION | 6   
Unmapped (Default value was set) -- POSCLPTL -> MIGRATION | 1,076   
Unmapped (Default value was set) -- POSCLREFERENCE -> MIGRATION | 263   
Unmapped (Default value was set) -- POSCLREPAIR -> MIGRATION | 2   
Unmapped (Default value was set) -- POSCLRESERVES -> MIGRATION | 1   
Unmapped (Default value was set) -- POSCLSMA -> MIGRATION | 1   
Unmapped (Default value was set) -- POSCLSPINNERS -> MIGRATION | 2,970   
Unmapped (Default value was set) -- POSCLST -> MIGRATION | 2   
Unmapped (Default value was set) -- POSCLSTACKS -> MIGRATION | 71,582   
Unmapped (Default value was set) -- POSCLUNKNOWN -> MIGRATION | 7   
Unmapped (Default value was set) -- POSYAAVAILSOON -> MIGRATION | 1   
Unmapped (Default value was set) -- POSYABINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- POSYACATALOGING -> MIGRATION | 2   
Unmapped (Default value was set) -- POSYALIB -> MIGRATION | 1   
Unmapped (Default value was set) -- POSYALIBCOLL -> MIGRATION | 35   
Unmapped (Default value was set) -- POSYAMEDIACTR -> MIGRATION | 1,459   
Unmapped (Default value was set) -- POSYAMMC -> MIGRATION | 10   
Unmapped (Default value was set) -- POSYAPERRACK -> MIGRATION | 5   
Unmapped (Default value was set) -- POSYAPTC -> MIGRATION | 2   
Unmapped (Default value was set) -- POSYAPTL -> MIGRATION | 1   
Unmapped (Default value was set) -- POSYAREFERENCE -> MIGRATION | 242   
Unmapped (Default value was set) -- POSYASPINNERS -> MIGRATION | 3,109   
Unmapped (Default value was set) -- POSYAST -> MIGRATION | 2   
Unmapped (Default value was set) -- POSYASTACKS -> MIGRATION | 31,737   
Unmapped (Default value was set) -- POSYAUNKNOWN -> MIGRATION | 12   
Unmapped (Default value was set) -- POSYAYAC -> MIGRATION | 1   
Unmapped (Default value was set) -- POSYAYMC -> MIGRATION | 1   
Unmapped (Default value was set) -- POSYAYNF -> MIGRATION | 1   
Unmapped (Default value was set) -- PTOBRL -> MIGRATION | 1   
Unmapped (Default value was set) -- PTOCATALOGING -> MIGRATION | 3   
Unmapped (Default value was set) -- PTOEAS -> MIGRATION | 827   
Unmapped (Default value was set) -- PTOJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- PTOJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- PTOLIBCOLL -> MIGRATION | 13   
Unmapped (Default value was set) -- PTOMEDIACTR -> MIGRATION | 2,099   
Unmapped (Default value was set) -- PTOMMC -> MIGRATION | 6   
Unmapped (Default value was set) -- PTOPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- PTOPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- PTOPTL -> MIGRATION | 79   
Unmapped (Default value was set) -- PTOREFERENCE -> MIGRATION | 85   
Unmapped (Default value was set) -- PTOSPINNERS -> MIGRATION | 1,926   
Unmapped (Default value was set) -- PTOSTACKS -> MIGRATION | 20,131   
Unmapped (Default value was set) -- RIOBINDERY -> MIGRATION | 11   
Unmapped (Default value was set) -- RIOCATALOGING -> MIGRATION | 2   
Unmapped (Default value was set) -- RIOEAS -> MIGRATION | 654   
Unmapped (Default value was set) -- RIOLIBCOLL -> MIGRATION | 11   
Unmapped (Default value was set) -- RIOMEDIACTR -> MIGRATION | 2,305   
Unmapped (Default value was set) -- RIOMMC -> MIGRATION | 4   
Unmapped (Default value was set) -- RIOPERRACK -> MIGRATION | 3   
Unmapped (Default value was set) -- RIOPTL -> MIGRATION | 52   
Unmapped (Default value was set) -- RIOREFERENCE -> MIGRATION | 104   
Unmapped (Default value was set) -- RIOSMA -> MIGRATION | 2   
Unmapped (Default value was set) -- RIOSPINNERS -> MIGRATION | 2,984   
Unmapped (Default value was set) -- RIOSTACKS -> MIGRATION | 15,876   
Unmapped (Default value was set) -- RIOSTC -> MIGRATION | 1   
Unmapped (Default value was set) -- RIOUNKNOWN -> MIGRATION | 8   
Unmapped (Default value was set) -- ROXBINDERY -> MIGRATION | 43   
Unmapped (Default value was set) -- ROXDAMAGED -> MIGRATION | 1   
Unmapped (Default value was set) -- ROXDISCARD -> MIGRATION | 962   
Unmapped (Default value was set) -- ROXEAS -> MIGRATION | 663   
Unmapped (Default value was set) -- ROXMEDIACTR -> MIGRATION | 199   
Unmapped (Default value was set) -- ROXREFERENCE -> MIGRATION | 61   
Unmapped (Default value was set) -- ROXREPAIR -> MIGRATION | 68   
Unmapped (Default value was set) -- ROXRES -> MIGRATION | 6   
Unmapped (Default value was set) -- ROXRESERVES -> MIGRATION | 14   
Unmapped (Default value was set) -- ROXSPINNERS -> MIGRATION | 5   
Unmapped (Default value was set) -- ROXSTACKS -> MIGRATION | 10,871   
Unmapped (Default value was set) -- ROXSTORAGE -> MIGRATION | 419   
Unmapped (Default value was set) -- ROXWITHDRAWN -> MIGRATION | 2,636   
Unmapped (Default value was set) -- SAJBRL -> MIGRATION | 2   
Unmapped (Default value was set) -- SAJDISCARD -> MIGRATION | 1   
Unmapped (Default value was set) -- SAJEAS -> MIGRATION | 812   
Unmapped (Default value was set) -- SAJJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- SAJLIBCOLL -> MIGRATION | 21   
Unmapped (Default value was set) -- SAJMEDIACTR -> MIGRATION | 2,183   
Unmapped (Default value was set) -- SAJMMC -> MIGRATION | 9   
Unmapped (Default value was set) -- SAJPERRACK -> MIGRATION | 5   
Unmapped (Default value was set) -- SAJPTC -> MIGRATION | 4   
Unmapped (Default value was set) -- SAJPTL -> MIGRATION | 56   
Unmapped (Default value was set) -- SAJREFERENCE -> MIGRATION | 186   
Unmapped (Default value was set) -- SAJSPINNERS -> MIGRATION | 2,015   
Unmapped (Default value was set) -- SAJSTACKS -> MIGRATION | 23,018   
Unmapped (Default value was set) -- SAJUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- SAJWITHDRAWN -> MIGRATION | 1   
Unmapped (Default value was set) -- SCAAFI -> MIGRATION | 5   
Unmapped (Default value was set) -- SCAANF -> MIGRATION | 79   
Unmapped (Default value was set) -- SCAANR -> MIGRATION | 18   
Unmapped (Default value was set) -- SCABINDERY -> MIGRATION | 7   
Unmapped (Default value was set) -- SCABRL -> MIGRATION | 3,771   
Unmapped (Default value was set) -- SCACLBINDERY -> MIGRATION | 3   
Unmapped (Default value was set) -- SCACLBRL -> MIGRATION | 913   
Unmapped (Default value was set) -- SCACLDAMAGED -> MIGRATION | 74   
Unmapped (Default value was set) -- SCACLDISCARD -> MIGRATION | 1,936   
Unmapped (Default value was set) -- SCACLEAS -> MIGRATION | 2,907   
Unmapped (Default value was set) -- SCACLLOST -> MIGRATION | 5   
Unmapped (Default value was set) -- SCACLLOSTPAID -> MIGRATION | 97   
Unmapped (Default value was set) -- SCACLMEDIACTR -> MIGRATION | 70   
Unmapped (Default value was set) -- SCACLPTL -> MIGRATION | 326   
Unmapped (Default value was set) -- SCACLREFERENCE -> MIGRATION | 129   
Unmapped (Default value was set) -- SCACLREPAIR -> MIGRATION | 25   
Unmapped (Default value was set) -- SCACLRES -> MIGRATION | 329   
Unmapped (Default value was set) -- SCACLSTACKS -> MIGRATION | 15,875   
Unmapped (Default value was set) -- SCACLSTORAGE -> MIGRATION | 26   
Unmapped (Default value was set) -- SCACLTES -> MIGRATION | 4   
Unmapped (Default value was set) -- SCACLWITHDRAWN -> MIGRATION | 3,905   
Unmapped (Default value was set) -- SCADAMAGED -> MIGRATION | 19   
Unmapped (Default value was set) -- SCADISCARD -> MIGRATION | 3,005   
Unmapped (Default value was set) -- SCAEAS -> MIGRATION | 13   
Unmapped (Default value was set) -- SCAINTRANSIT -> MIGRATION | 2   
Unmapped (Default value was set) -- SCAJFI -> MIGRATION | 11   
Unmapped (Default value was set) -- SCAJNF -> MIGRATION | 28   
Unmapped (Default value was set) -- SCALIBCOLL -> MIGRATION | 196   
Unmapped (Default value was set) -- SCALOST -> MIGRATION | 2   
Unmapped (Default value was set) -- SCALOSTPAID -> MIGRATION | 35   
Unmapped (Default value was set) -- SCAMEDIACTR -> MIGRATION | 198   
Unmapped (Default value was set) -- SCAMISSING -> MIGRATION | 3   
Unmapped (Default value was set) -- SCAREFERENCE -> MIGRATION | 312   
Unmapped (Default value was set) -- SCAREPAIR -> MIGRATION | 15   
Unmapped (Default value was set) -- SCARES -> MIGRATION | 3,871   
Unmapped (Default value was set) -- SCARESERVES -> MIGRATION | 2   
Unmapped (Default value was set) -- SCASPINNERS -> MIGRATION | 5   
Unmapped (Default value was set) -- SCASTACKS -> MIGRATION | 35,205   
Unmapped (Default value was set) -- SCASTORAGE -> MIGRATION | 626   
Unmapped (Default value was set) -- SCATES -> MIGRATION | 4   
Unmapped (Default value was set) -- SCAWITHDRAWN -> MIGRATION | 1,703   
Unmapped (Default value was set) -- SCAYABRL -> MIGRATION | 929   
Unmapped (Default value was set) -- SCAYADAMAGED -> MIGRATION | 6   
Unmapped (Default value was set) -- SCAYADISCARD -> MIGRATION | 987   
Unmapped (Default value was set) -- SCAYALOST -> MIGRATION | 2   
Unmapped (Default value was set) -- SCAYALOSTPAID -> MIGRATION | 2   
Unmapped (Default value was set) -- SCAYAMEDIACTR -> MIGRATION | 55   
Unmapped (Default value was set) -- SCAYAREFERENCE -> MIGRATION | 170   
Unmapped (Default value was set) -- SCAYARES -> MIGRATION | 38   
Unmapped (Default value was set) -- SCAYASPINNERS -> MIGRATION | 2   
Unmapped (Default value was set) -- SCAYASTACKS -> MIGRATION | 15,245   
Unmapped (Default value was set) -- SCAYASTORAGE -> MIGRATION | 342   
Unmapped (Default value was set) -- SCAYATES -> MIGRATION | 4   
Unmapped (Default value was set) -- SCAYAUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- SCAYAWITHDRAWN -> MIGRATION | 2,051   
Unmapped (Default value was set) -- SCAYFI -> MIGRATION | 30   
Unmapped (Default value was set) -- SCAYNF -> MIGRATION | 1   
Unmapped (Default value was set) -- SGEEAS -> MIGRATION | 1,022   
Unmapped (Default value was set) -- SGEJFI -> MIGRATION | 1   
Unmapped (Default value was set) -- SGEJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- SGEJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- SGELIBCOLL -> MIGRATION | 22   
Unmapped (Default value was set) -- SGEMAC -> MIGRATION | 1   
Unmapped (Default value was set) -- SGEMEDIACTR -> MIGRATION | 3,052   
Unmapped (Default value was set) -- SGEMMC -> MIGRATION | 9   
Unmapped (Default value was set) -- SGEPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- SGEPTC -> MIGRATION | 2   
Unmapped (Default value was set) -- SGEPTL -> MIGRATION | 70   
Unmapped (Default value was set) -- SGEREFERENCE -> MIGRATION | 144   
Unmapped (Default value was set) -- SGESPINNERS -> MIGRATION | 4,076   
Unmapped (Default value was set) -- SGEST -> MIGRATION | 1   
Unmapped (Default value was set) -- SGESTACKS -> MIGRATION | 26,682   
Unmapped (Default value was set) -- SGESTORAGE -> MIGRATION | 1   
Unmapped (Default value was set) -- SGEUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- SIPAMC -> MIGRATION | 56   
Unmapped (Default value was set) -- SIPEAS -> MIGRATION | 744   
Unmapped (Default value was set) -- SIPJMC -> MIGRATION | 2   
Unmapped (Default value was set) -- SIPJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- SIPLIBCOLL -> MIGRATION | 10   
Unmapped (Default value was set) -- SIPMEDIACTR -> MIGRATION | 2,046   
Unmapped (Default value was set) -- SIPMMC -> MIGRATION | 6   
Unmapped (Default value was set) -- SIPPERRACK -> MIGRATION | 3   
Unmapped (Default value was set) -- SIPPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- SIPPTL -> MIGRATION | 76   
Unmapped (Default value was set) -- SIPREFERENCE -> MIGRATION | 199   
Unmapped (Default value was set) -- SIPSPINNERS -> MIGRATION | 1,459   
Unmapped (Default value was set) -- SIPST -> MIGRATION | 1   
Unmapped (Default value was set) -- SIPSTACKS -> MIGRATION | 20,192   
Unmapped (Default value was set) -- SIPSTE -> MIGRATION | 2   
Unmapped (Default value was set) -- SIPSTORAGE -> MIGRATION | 1   
Unmapped (Default value was set) -- SIPUNKNOWN -> MIGRATION | 10   
Unmapped (Default value was set) -- SIPYMC -> MIGRATION | 8   
Unmapped (Default value was set) -- SJSEAS -> MIGRATION | 4   
Unmapped (Default value was set) -- SJSMEDIACTR -> MIGRATION | 786   
Unmapped (Default value was set) -- SJSMMC -> MIGRATION | 1   
Unmapped (Default value was set) -- SJSPERRACK -> MIGRATION | 2   
Unmapped (Default value was set) -- SJSPTL -> MIGRATION | 11   
Unmapped (Default value was set) -- SJSREFERENCE -> MIGRATION | 25   
Unmapped (Default value was set) -- SJSSPINNERS -> MIGRATION | 532   
Unmapped (Default value was set) -- SJSSTACKS -> MIGRATION | 3,142   
Unmapped (Default value was set) -- SJSUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- SMSMEDIACTR -> MIGRATION | 97   
Unmapped (Default value was set) -- SMSPERRACK -> MIGRATION | 2   
Unmapped (Default value was set) -- SMSREFERENCE -> MIGRATION | 8   
Unmapped (Default value was set) -- SMSSPINNERS -> MIGRATION | 108   
Unmapped (Default value was set) -- SMSSTACKS -> MIGRATION | 935   
Unmapped (Default value was set) -- SMSUNKNOWN -> MIGRATION | 2   
Unmapped (Default value was set) -- STHEAS -> MIGRATION | 589   
Unmapped (Default value was set) -- STHJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- STHJNF -> MIGRATION | 1   
Unmapped (Default value was set) -- STHLIBCOLL -> MIGRATION | 1   
Unmapped (Default value was set) -- STHMEDIACTR -> MIGRATION | 1,995   
Unmapped (Default value was set) -- STHMMC -> MIGRATION | 10   
Unmapped (Default value was set) -- STHPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- STHPTC -> MIGRATION | 1   
Unmapped (Default value was set) -- STHPTL -> MIGRATION | 39   
Unmapped (Default value was set) -- STHREFERENCE -> MIGRATION | 81   
Unmapped (Default value was set) -- STHSPINNERS -> MIGRATION | 1,924   
Unmapped (Default value was set) -- STHSTACKS -> MIGRATION | 18,835   
Unmapped (Default value was set) -- STHUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- STJBINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- STJBRL -> MIGRATION | 2   
Unmapped (Default value was set) -- STJCATALOGING -> MIGRATION | 1   
Unmapped (Default value was set) -- STJEAS -> MIGRATION | 1,027   
Unmapped (Default value was set) -- STJJNF -> MIGRATION | 3   
Unmapped (Default value was set) -- STJLIBCOLL -> MIGRATION | 34   
Unmapped (Default value was set) -- STJMAP -> MIGRATION | 1   
Unmapped (Default value was set) -- STJMEDIACTR -> MIGRATION | 2,710   
Unmapped (Default value was set) -- STJMMC -> MIGRATION | 9   
Unmapped (Default value was set) -- STJPERRACK -> MIGRATION | 5   
Unmapped (Default value was set) -- STJPTC -> MIGRATION | 2   
Unmapped (Default value was set) -- STJPTL -> MIGRATION | 68   
Unmapped (Default value was set) -- STJREFERENCE -> MIGRATION | 118   
Unmapped (Default value was set) -- STJSPINNERS -> MIGRATION | 3,880   
Unmapped (Default value was set) -- STJST -> MIGRATION | 1   
Unmapped (Default value was set) -- STJSTACKS -> MIGRATION | 26,075   
Unmapped (Default value was set) -- STJUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- STJWITHDRAWN -> MIGRATION | 1   
Unmapped (Default value was set) -- TESBINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- TESCATALOGING -> MIGRATION | 6   
Unmapped (Default value was set) -- TESDAMAGED -> MIGRATION | 8   
Unmapped (Default value was set) -- TESDISCARD -> MIGRATION | 1   
Unmapped (Default value was set) -- TESEAS -> MIGRATION | 21   
Unmapped (Default value was set) -- TESINTRANSIT -> MIGRATION | 1   
Unmapped (Default value was set) -- TESLIB -> MIGRATION | 2   
Unmapped (Default value was set) -- TESLIBCOLL -> MIGRATION | 229   
Unmapped (Default value was set) -- TESMEDIACTR -> MIGRATION | 23   
Unmapped (Default value was set) -- TESMMC -> MIGRATION | 1   
Unmapped (Default value was set) -- TESPERRACK -> MIGRATION | 9   
Unmapped (Default value was set) -- TESPTC -> MIGRATION | 199   
Unmapped (Default value was set) -- TESREFERENCE -> MIGRATION | 106   
Unmapped (Default value was set) -- TESRES -> MIGRATION | 1   
Unmapped (Default value was set) -- TESRESERVES -> MIGRATION | 1   
Unmapped (Default value was set) -- TESSPINNERS -> MIGRATION | 9   
Unmapped (Default value was set) -- TESSTACKS -> MIGRATION | 514   
Unmapped (Default value was set) -- TESSTORAGE -> MIGRATION | 1,203   
Unmapped (Default value was set) -- TESTES -> MIGRATION | 21   
Unmapped (Default value was set) -- TESUNKNOWN -> MIGRATION | 14,227   
Unmapped (Default value was set) -- TESWITHDRAWN -> MIGRATION | 3   
Unmapped (Default value was set) -- TGODAMAGED -> MIGRATION | 1   
Unmapped (Default value was set) -- TGODISCARD -> MIGRATION | 6,957   
Unmapped (Default value was set) -- TGOEAS -> MIGRATION | 1   
Unmapped (Default value was set) -- TGOSTACKS -> MIGRATION | 14   
Unmapped (Default value was set) -- THLBINDERY -> MIGRATION | 732   
Unmapped (Default value was set) -- THLDISCARD -> MIGRATION | 12   
Unmapped (Default value was set) -- THLREFERENCE -> MIGRATION | 5   
Unmapped (Default value was set) -- THLREPAIR -> MIGRATION | 258   
Unmapped (Default value was set) -- THLRES -> MIGRATION | 1,889   
Unmapped (Default value was set) -- THLSTACKS -> MIGRATION | 8,583   
Unmapped (Default value was set) -- THLWITHDRAWN -> MIGRATION | 8   
Unmapped (Default value was set) -- TUNCATALOGING -> MIGRATION | 2   
Unmapped (Default value was set) -- TUNEAS -> MIGRATION | 1,068   
Unmapped (Default value was set) -- TUNEIC -> MIGRATION | 318   
Unmapped (Default value was set) -- TUNJMC -> MIGRATION | 1   
Unmapped (Default value was set) -- TUNJNF -> MIGRATION | 3   
Unmapped (Default value was set) -- TUNLIBCOLL -> MIGRATION | 82   
Unmapped (Default value was set) -- TUNMEDIACTR -> MIGRATION | 3,104   
Unmapped (Default value was set) -- TUNMMC -> MIGRATION | 22   
Unmapped (Default value was set) -- TUNPERRACK -> MIGRATION | 10   
Unmapped (Default value was set) -- TUNPTC -> MIGRATION | 3   
Unmapped (Default value was set) -- TUNPTL -> MIGRATION | 112   
Unmapped (Default value was set) -- TUNRBC -> MIGRATION | 1   
Unmapped (Default value was set) -- TUNREFERENCE -> MIGRATION | 94   
Unmapped (Default value was set) -- TUNSPINNERS -> MIGRATION | 2,698   
Unmapped (Default value was set) -- TUNSTACKS -> MIGRATION | 31,461   
Unmapped (Default value was set) -- TUNSTE -> MIGRATION | 68   
Unmapped (Default value was set) -- TUNUNKNOWN -> MIGRATION | 27   
Unmapped (Default value was set) -- WPCBINDERY -> MIGRATION | 1   
Unmapped (Default value was set) -- WPCMEDIACTR -> MIGRATION | 664   
Unmapped (Default value was set) -- WPCPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- WPCPTL -> MIGRATION | 2   
Unmapped (Default value was set) -- WPCREFERENCE -> MIGRATION | 40   
Unmapped (Default value was set) -- WPCSPINNERS -> MIGRATION | 990   
Unmapped (Default value was set) -- WPCSTACKS -> MIGRATION | 3,576   
Unmapped (Default value was set) -- WPCUNKNOWN -> MIGRATION | 1   
Unmapped (Default value was set) -- YTCEAS -> MIGRATION | 2   
Unmapped (Default value was set) -- YTCMEDIACTR -> MIGRATION | 650   
Unmapped (Default value was set) -- YTCPERRACK -> MIGRATION | 4   
Unmapped (Default value was set) -- YTCPTL -> MIGRATION | 8   
Unmapped (Default value was set) -- YTCREFERENCE -> MIGRATION | 37   
Unmapped (Default value was set) -- YTCSPINNERS -> MIGRATION | 667   
Unmapped (Default value was set) -- YTCSTACKS -> MIGRATION | 5,509   
Unmapped (Default value was set) -- YTCSTC -> MIGRATION | 1   
Unmapped (Default value was set) -- YTCUNKNOWN -> MIGRATION | 3   
Unmapped (Default value was set) -- YTCYNF -> MIGRATION | 2   
</details>   
   
## Suppression    
What records got assigned what suppression setting in the records.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Suppressed from discovery = False | 1,180,521   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 1,180,521 (100%) 
accessionNumber | 0 (0%) | 1,180,521 (100%) 
administrativeNotes | 0 (0%) | 1,180,521 (100%) 
barcode | 1,180,521 (100%) | 0 (0%) 
chronology | 0 (0%) | 1,180,521 (100%) 
circulationNotes | 0 (0%) | 1,180,521 (100%) 
copyNumber | 1,180,521 (100%) | 0 (0%) 
descriptionOfPieces | 1,821 (0%) | 1,178,700 (100%) 
discoverySuppress | 1,180,521 (100%) | 0 (0%) 
effectiveCallNumberComponents | 0 (0%) | 1,180,521 (100%) 
effectiveLocationId | 0 (0%) | 1,180,521 (100%) 
effectiveShelvingOrder | 0 (0%) | 1,180,521 (100%) 
electronicAccess | 0 (0%) | 1,180,521 (100%) 
enumeration | 0 (0%) | 1,180,521 (100%) 
formerIds | 1,180,521 (100%) | 0 (0%) 
holdingsRecord2 | 0 (0%) | 1,180,521 (100%) 
holdingsRecordId | 1,180,521 (100%) | 0 (0%) 
hrid | 0 (0%) | 1,180,521 (100%) 
id | 1,180,521 (100%) | 0 (0%) 
inTransitDestinationServicePointId | 0 (0%) | 1,180,521 (100%) 
itemDamagedStatusDate | 0 (0%) | 1,180,521 (100%) 
itemDamagedStatusId | 0 (0%) | 1,180,521 (100%) 
itemIdentifier | 1,180,521 (100%) | 0 (0%) 
itemLevelCallNumber | 0 (0%) | 1,180,521 (100%) 
itemLevelCallNumberPrefix | 0 (0%) | 1,180,521 (100%) 
itemLevelCallNumberSuffix | 0 (0%) | 1,180,521 (100%) 
itemLevelCallNumberTypeId | 1,180,521 (100%) | 0 (0%) 
lastCheckIn | 0 (0%) | 1,180,521 (100%) 
materialType | 0 (0%) | 1,180,521 (100%) 
materialTypeId | 1,180,521 (100%) | 0 (0%) 
metadata | 1,180,521 (100%) | 0 (0%) 
metadata.createdByUserId | 1,180,521 (100%) | 0 (0%) 
metadata.createdDate | 1,180,521 (100%) | 0 (0%) 
metadata.updatedByUserId | 1,180,521 (100%) | 0 (0%) 
metadata.updatedDate | 1,180,521 (100%) | 0 (0%) 
missingPieces | 0 (0%) | 1,180,521 (100%) 
missingPiecesDate | 0 (0%) | 1,180,521 (100%) 
notes | 1,180,521 (100%) | 0 (0%) 
notes.itemNoteTypeId | 1,180,521 (100%) | 0 (0%) 
notes.note | 1,180,521 (100%) | 0 (0%) 
numberOfMissingPieces | 0 (0%) | 1,180,521 (100%) 
numberOfPieces | 1,821 (0%) | 1,178,700 (100%) 
permanentLoanTypeId | 1,180,521 (100%) | 0 (0%) 
permanentLocation | 0 (0%) | 1,180,521 (100%) 
permanentLocationId | 1,180,521 (100%) | 0 (0%) 
purchaseOrderLineIdentifier | 0 (0%) | 1,180,521 (100%) 
statisticalCodeIds | 0 (0%) | 1,180,521 (100%) 
status | 1,180,521 (100%) | 0 (0%) 
status.date | 1,180,521 (100%) | 0 (0%) 
status.name | 1,180,521 (100%) | 0 (0%) 
tags | 0 (0%) | 1,180,521 (100%) 
temporaryLoanTypeId | 0 (0%) | 1,180,521 (100%) 
temporaryLocation | 0 (0%) | 1,180,521 (100%) 
temporaryLocationId | 0 (0%) | 1,180,521 (100%) 
volume | 0 (0%) | 1,180,521 (100%) 
yearCaption | 0 (0%) | 1,180,521 (100%) 
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
acquisitionDate | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
barcodeNumber | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
callNumbertype | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
copy | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
dateInventoried | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
holdingId | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
homeLocation | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
itemCategory | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
itemCategory2 | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
itemId | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
itemsNotescomment | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
loantype | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
mtype | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
numberPieces | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
priceNote | 2,361,042 (200.0%) | 2,361,042 (200%) | 0  
volumen | 1,180,521 (100.0%) | 1,180,521 (100%) | 0  
</details>   
