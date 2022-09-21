# Loans migration report   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
## Timings   
   
Measure | Value   
--- | ---:   
Time Started: | 2022-09-20T21:14:48.337309+00:00   
Time Finished: | 2022-09-20T21:15:04.116030+00:00   
Elapsed time: | 0:00:15.778721   
   
## Details    
    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
Check out must be performed at a service point | 9   
Hour and minute not specified for due date. Assuming end of local calendar day (23:59)... | 1   
Other checkout failure: Check out must be performed at a service point | 9   
Provided due_date is not UTC, setting tzinfo to tenant timezone (UTC) | 17   
Provided out_date is not UTC, setting tzinfo to tenant timezone (UTC) | 17   
</details>   
   
## General statistics    
A list of general counters to outline the transformation as a whole.    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Discarded Loans | 5   
Failed loans | 16   
Loans verified against migrated user and item | 9   
Processed loans | 9   
</details>   
   
## Discarded loans    
List of loans discarded for various resons    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
Empty properties in legacy data - patron_barcode | 1   
Loans discarded. Had migrated item barcode: False. Had migrated user barcode: False | 1   
Loans discarded. Had migrated item barcode: False. Had migrated user barcode: True | 2   
Not an allowed status - Missing | 3   
Time alignment issues - both dates | 1   
</details>   
