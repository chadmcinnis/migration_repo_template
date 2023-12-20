# Bibliographic records transformation report   
<br/>Data errors preventing records from being migrated are marked **FIX BEFORE MIGRATION**. The library is advised to clean up these errors in the source data.<br/><br/> The sections related to field counts and mapping results are marked **REVIEW**. These do not indicate errors preventing records from being migrated, but may point to data anomalies or in the mappings. The library should review these to make sure that the numbers are what one would expect, knowing the source data. Is this the expected number of serials? Is this the expected number of cartographic materials?
## Timings   
   
Measure | Value   
--- | ---:   
Time Started: | 2023-12-20T01:57:49.758271+00:00   
Time Finished: | 2023-12-20T02:07:04.497689+00:00   
Elapsed time: | 0:09:14.739418   
   
## General statistics    
A list of general counters to outline the transformation as a whole.    
<details><summary>Click to expand all 10 things</summary>     
   
Measure | Count   
--- | ---:   
Duplicate MARC record identifiers  | 30   
Failed records. No unique record identifiers in legacy record | 30   
Inventory records written to disk | 162,949   
Records in file before parsing | 162,984   
Records successfully decoded from MARC21 | 162,983   
Records that failed transformation. Check log for details | 35   
Records with encoding errors - parsing failed | 1   
SRS records written to disk | 162,949   
Unique ID:s written to legacy map | 162,949   
</details>   
   
## HRID and 001/035 handling    
There are two ways of handling HRIDs. The default behaviour is to take the current 001 and move that to a new 035. This will also emerge as an Identifier on the Inventory Instances. The 001 and Instance HRID will be generated from the HRID settings in FOLIO. The second option is to maintain the 001s in the records, and also add this as the Instance HRID    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
Added 035 from 001 | 162,983   
Created HRID using default settings | 162,983   
Values in 003: SIRSI | 162,983   
</details>   
   
## Record status (leader pos 5)    
Library action: **All values that are not a, c, d, n or p will be set to c. If this is not what you want, you need to correct these values in your system. **<br/>An overview of the Record statuses (Leader position 5) present in your source data.    Pay attention to the number of occurrences of the value 'd'. These d's are expressing that they are deleted, and the records might not work as expected in FOLIO. Consider marking them as suppressed in your current system and export them as a separate batch in order to have them suppressed in FOLIO. Allowed values according to the MARC standard are a,c,d,n,p    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
Original value: a | 169   
Original value: c | 120,836   
Original value: n | 40,667   
Original value: p | 1,311   
</details>   
   
## Trivia    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Total number of Tags processed | 5,560,192   
</details>   
   
## Mapped identifier types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Identifier type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 22 things</summary>     
   
Measure | Count   
--- | ---:   
010 -> LCCN | 81,609   
019 -> Cancelled system control number | 6,439   
020 -> ISBN | 214,686   
020 -> Invalid ISBN | 1,050   
022 -> ISSN | 361   
022 -> Invalid ISSN | 35   
022 -> Linking ISSN | 73   
024 -> ISMN | 2,554   
024 -> Invalid ISMN | 30   
024 -> Invalid UPC | 30   
024 -> Other standard identifier | 2,583   
024 -> UPC | 2,554   
028 -> Publisher or distributor number | 3,834   
035 -> Cancelled system control number | 33,342   
035 -> OCLC | 65,744   
035 -> System control number | 168,635   
074 -> GPO item number | 5   
780 -> ISBN | 197   
780 -> ISSN | 197   
785 -> ISBN | 83   
785 -> ISSN | 83   
</details>   
   
## Mapped classification types    
    
<details><summary>Click to expand all 6 things</summary>     
   
Measure | Count   
--- | ---:   
Dewey | 21,221   
GDC | 15   
LC | 46,565   
NLM | 510   
UDC | 21   
</details>   
   
## Mapped contributor name types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Name type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 11 things</summary>     
   
Measure | Count   
--- | ---:   
100 -> Personal name | 137,660   
110 -> Corporate name | 3,609   
111 -> Meeting name | 236   
700 -> Personal name | 96,636   
710 -> Corporate name | 15,497   
711 -> Meeting name | 270   
720 -> Corporate name | 75   
720 -> Personal name | 150   
880 -> Corporate name | 23   
880 -> Personal name | 61   
</details>   
   
## Matched Modes of issuance code    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Mode of issuace values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
integrating resource -- 4fc0f4fe-06fd-490a-a078-c4da1754e03a | 3   
serial -- 068b5344-e2a6-40df-9186-1829e13cd344 | 1,036   
single unit -- 9d18a02f-5897-4c31-9106-c9abb5c7ae8b | 161,944   
</details>   
   
## Language codes in records    
A breakdown of language codes occuring in the records. Purely informational.    
<details><summary>Click to expand all 167 things</summary>     
   
Measure | Count   
--- | ---:   
    | 229   
  g | 1   
 eg | 1   
 en | 3   
+ng | 1   
ach | 1   
afr | 10   
amh | 4   
and | 4   
ang | 4   
ara | 140   
arc | 2   
arm | 1   
ath | 2   
awa | 1   
aze | 1   
baq | 3   
ben | 16   
bho | 1   
bik | 1   
bnt | 1   
bra | 1   
bre | 1   
bul | 3   
bur | 1   
cai | 1   
cam | 1   
cat | 7   
chi | 247   
chu | 1   
cop | 1   
cpe | 18   
cpf | 18   
crp | 6   
cze | 16   
d   | 6   
dak | 1   
dan | 42   
dua | 1   
dut | 103   
dyu | 1   
ebg | 1   
egy | 2   
emg | 2   
emn | 2   
en0 | 1   
end | 5   
enf | 10   
eng | 160,217   
enh | 2   
enk | 77   
enm | 3   
enn | 5   
ent | 3   
esp | 1   
est | 4   
eth | 2   
fil | 1   
fin | 5   
fr  | 3   
fre | 1,693   
frm | 1   
gae | 2   
geo | 1   
ger | 513   
gla | 1   
gle | 2   
glg | 1   
got | 1   
grc | 39   
gre | 9   
guj | 8   
hat | 4   
hau | 5   
haw | 3   
heb | 43   
hih | 1   
hin | 387   
hrv | 1   
hun | 9   
ibo | 2   
ice | 2   
iku | 1   
inc | 2   
ind | 10   
ita | 262   
jav | 1   
jpn | 544   
jpr | 1   
kam | 1   
kan | 3   
kau | 1   
kha | 1   
kik | 2   
kor | 92   
kur | 1   
lat | 39   
lav | 4   
lit | 1   
mac | 1   
mal | 1   
man | 3   
mar | 4   
may | 3   
men | 1   
mos | 1   
mul | 80   
nah | 2   
nav | 2   
nep | 2   
nic | 2   
nor | 36   
nya | 1   
pal | 1   
pan | 6   
pap | 2   
per | 27   
pli | 3   
pol | 10   
por | 194   
pus | 1   
que | 1   
ren | 1   
roa | 3   
rum | 5   
rus | 101   
sai | 6   
san | 42   
scc | 1   
sco | 2   
scr | 4   
sgn | 11   
sho | 1   
slo | 2   
sng | 1   
som | 2   
sp  | 2   
spa | 3,506   
ssa | 1   
sso | 2   
sux | 1   
swa | 16   
swe | 72   
tam | 3   
tel | 6   
tgl | 1   
tha | 19   
tib | 13   
tlh | 1   
tne | 1   
tsw | 1   
tuk | 1   
tur | 11   
twi | 1   
ukr | 1   
und | 93   
urd | 21   
vie | 7   
wel | 4   
xho | 5   
yid | 2   
yor | 23   
zul | 2   
zxx | 36   
|   | 2   
||| | 2   
</details>   
   
## Suppression    
What records got assigned what suppression setting in the records.    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
Staff suppressed = False  | 162,983   
Suppressed from discovery = False | 162,983   
</details>   
   
## Authorization sources and related information    
    
<details><summary>Click to expand all 390 things</summary>     
   
Measure | Count   
--- | ---:   
$0 base uri or source code: AW3 | 13   
$0 base uri or source code: DE-101 | 1   
$0 base uri or source code: DE-588 | 11   
$0 base uri or source code: DE-588c | 2   
$0 base uri or source code: DE-601 | 1   
$0 base uri or source code: KCLS | 1   
$0 base uri or source code: LARL_NWRL_CONSORTIUM | 2   
$0 base uri or source code: NL-LeOCL | 9   
$0 base uri or source code: OCoLC | 5,109   
$0 base uri or source code: RC9 | 4   
$0 base uri or source code: http://id.loc.gov | 1   
$0 base uri or source code: http://rdaregistry.info | 1   
$0 base uri or source code: local | 6   
Source of heading or term:  | 1,315   
Source of heading or term: (paperback) | 1   
Source of heading or term: 0 | 19   
Source of heading or term: 0.01.2007 | 1   
Source of heading or term: 001 | 1   
Source of heading or term: 004 | 1   
Source of heading or term: 006. | 1   
Source of heading or term: 007 | 2   
Source of heading or term: 007, | 1   
Source of heading or term: 008, | 2   
Source of heading or term: 008- | 1   
Source of heading or term: 010 | 1   
Source of heading or term: 010, | 2   
Source of heading or term: 012 | 2   
Source of heading or term: 012. | 1   
Source of heading or term: 014 | 1   
Source of heading or term: 014, | 2   
Source of heading or term: 02 | 1   
Source of heading or term: 0cm | 2   
Source of heading or term: 0cm. | 2   
Source of heading or term: 1 | 81   
Source of heading or term: 11 | 10   
Source of heading or term: 12 | 19   
Source of heading or term: 121 | 1   
Source of heading or term: 12A | 1   
Source of heading or term: 13 | 23   
Source of heading or term: 14 | 33   
Source of heading or term: 15 | 3   
Source of heading or term: 17 | 1   
Source of heading or term: 18 | 72   
Source of heading or term: 19 | 1,237   
Source of heading or term: 1c | 1   
Source of heading or term: 1csh | 3   
Source of heading or term: 2 | 88   
Source of heading or term: 2. | 1   
Source of heading or term: 2.07.2002 | 1   
Source of heading or term: 2.11.96 | 1   
Source of heading or term: 20 | 2,286   
Source of heading or term: 2000 | 2   
Source of heading or term: 2001 | 3   
Source of heading or term: 2002 | 2   
Source of heading or term: 2003 | 2   
Source of heading or term: 2004 | 2   
Source of heading or term: 2005 | 1   
Source of heading or term: 2006 | 3   
Source of heading or term: 2007 | 8   
Source of heading or term: 2008 | 9   
Source of heading or term: 2009 | 6   
Source of heading or term: 2009, | 1   
Source of heading or term: 2009. | 1   
Source of heading or term: 201 | 1   
Source of heading or term: 2010 | 11   
Source of heading or term: 2010. | 2   
Source of heading or term: 2011 | 7   
Source of heading or term: 2012 | 16   
Source of heading or term: 2012. | 1   
Source of heading or term: 2013 | 7   
Source of heading or term: 2014 | 6   
Source of heading or term: 2014. | 1   
Source of heading or term: 2015 | 8   
Source of heading or term: 2015. | 1   
Source of heading or term: 2016 | 3   
Source of heading or term: 2017 | 2   
Source of heading or term: 2017. | 1   
Source of heading or term: 2018. | 1   
Source of heading or term: 2019 | 1   
Source of heading or term: 202 | 1   
Source of heading or term: 2020 | 1   
Source of heading or term: 2020. | 2   
Source of heading or term: 2021 | 2   
Source of heading or term: 2021. | 1   
Source of heading or term: 2022 | 1   
Source of heading or term: 2022. | 1   
Source of heading or term: 21 | 52,089   
Source of heading or term: 21. | 10   
Source of heading or term: 21.235 | 1   
Source of heading or term: 210 | 1   
Source of heading or term: 210920 | 1   
Source of heading or term: 211 | 2   
Source of heading or term: 212 | 3   
Source of heading or term: 213 | 1   
Source of heading or term: 214 | 1   
Source of heading or term: 219 | 1   
Source of heading or term: 21Di | 1   
Source of heading or term: 21` | 1   
Source of heading or term: 21d | 1   
Source of heading or term: 22 | 41,514   
Source of heading or term: 22 | 1   
Source of heading or term: 22. | 23   
Source of heading or term: 220 | 4   
Source of heading or term: 2208539228722 | 1   
Source of heading or term: 221 | 18   
Source of heading or term: 222 | 6   
Source of heading or term: 223 | 18   
Source of heading or term: 2230211107071380 | 1   
Source of heading or term: 227 | 1   
Source of heading or term: 22nd | 1   
Source of heading or term: 23 | 45,157   
Source of heading or term: 23. | 4   
Source of heading or term: 23J | 1   
Source of heading or term: 23` | 1   
Source of heading or term: 23g | 1   
Source of heading or term: 23i | 1   
Source of heading or term: 23m, | 1   
Source of heading or term: 23nb | 1   
Source of heading or term: 24 | 2   
Source of heading or term: 263 | 1   
Source of heading or term: 27 | 1   
Source of heading or term: 29. | 1   
Source of heading or term: 2c | 3   
Source of heading or term: 2cm. | 2   
Source of heading or term: 2d | 1   
Source of heading or term: 2rdacontent | 2   
Source of heading or term: 3 | 35   
Source of heading or term: 3. | 1   
Source of heading or term: 33 | 11   
Source of heading or term: 4 | 5   
Source of heading or term: 5 | 11   
Source of heading or term: 56 | 1   
Source of heading or term: 6 | 3   
Source of heading or term: 6cm | 2   
Source of heading or term: 7 | 2   
Source of heading or term: 7) | 2   
Source of heading or term: 730-7328 | 1   
Source of heading or term: 7cm | 1   
Source of heading or term: 8 | 4   
Source of heading or term: 8.09.2018 | 1   
Source of heading or term: 9 | 2   
Source of heading or term: Amazon | 1   
Source of heading or term: BISAC | 2   
Source of heading or term: DE-101 | 2   
Source of heading or term: DE-600 | 6   
Source of heading or term: DNLM | 70   
Source of heading or term: E21 | 1   
Source of heading or term: GyFmDB | 5   
Source of heading or term: HP | 1   
Source of heading or term: IsJJNL | 2   
Source of heading or term: J21 | 1   
Source of heading or term: JTNDL | 17   
Source of heading or term: LAC | 1   
Source of heading or term: NDC9 | 1   
Source of heading or term: NIPO | 3   
Source of heading or term: OverDrive | 19,089   
Source of heading or term: PF | 1   
Source of heading or term: TTSH. | 1   
Source of heading or term: Tin | 1   
Source of heading or term: UK | 9   
Source of heading or term: UK-WkNB | 3   
Source of heading or term: UNKNOWN | 1   
Source of heading or term: Uk | 520   
Source of heading or term: WISH | 1   
Source of heading or term: aat | 52   
Source of heading or term: ascl | 2   
Source of heading or term: bccb | 6   
Source of heading or term: bcl | 22   
Source of heading or term: bicssc | 9   
Source of heading or term: bidex | 402   
Source of heading or term: bidex. | 2   
Source of heading or term: bisacsh | 7,490   
Source of heading or term: bl | 3   
Source of heading or term: blmarc | 2   
Source of heading or term: blmsh | 3   
Source of heading or term: blsrissc | 1   
Source of heading or term: bnb | 2,017   
Source of heading or term: bwi | 1   
Source of heading or term: can | 4   
Source of heading or term: carrier | 1   
Source of heading or term: cct | 98   
Source of heading or term: cct. | 1   
Source of heading or term: childrens | 1   
Source of heading or term: clc | 2   
Source of heading or term: clc. | 1   
Source of heading or term: composer. | 1   
Source of heading or term: content | 6   
Source of heading or term: csh | 1   
Source of heading or term: damedia | 1   
Source of heading or term: dcs | 7   
Source of heading or term: de-600 | 1   
Source of heading or term: discsafrican | 1   
Source of heading or term: dnb | 8   
Source of heading or term: do | 1   
Source of heading or term: doi | 1   
Source of heading or term: ebgenr | 1   
Source of heading or term: eclas | 22   
Source of heading or term: edtf | 23   
Source of heading or term: eet | 1   
Source of heading or term: eflch | 17   
Source of heading or term: embne | 2   
Source of heading or term: ept | 1   
Source of heading or term: ericd | 2   
Source of heading or term: fast | 5,482   
Source of heading or term: fast. | 1   
Source of heading or term: fcps | 1   
Source of heading or term: flcgft | 4   
Source of heading or term: fsafd | 2   
Source of heading or term: g. | 1   
Source of heading or term: gasfd | 18   
Source of heading or term: gdafd | 3   
Source of heading or term: glcgft?UNAUTHORIZED | 1   
Source of heading or term: gnd | 69   
Source of heading or term: gsad | 1   
Source of heading or term: gsadf | 1   
Source of heading or term: gsaf | 1   
Source of heading or term: gsafd | 14,795   
Source of heading or term: gsafd. | 21   
Source of heading or term: gsald | 1   
Source of heading or term: gsfad | 8   
Source of heading or term: gsfd | 7   
Source of heading or term: gssfd | 1   
Source of heading or term: gtin-14 | 60   
Source of heading or term: gtlm | 1   
Source of heading or term: gtt | 131   
Source of heading or term: gttg | 9   
Source of heading or term: henn | 6   
Source of heading or term: http | 25   
Source of heading or term: http. | 4   
Source of heading or term: idsbb | 1   
Source of heading or term: idszbz | 15   
Source of heading or term: idszbzna | 2   
Source of heading or term: iso639-3 | 1   
Source of heading or term: jlabsh/3 | 1   
Source of heading or term: jpnmarc | 8   
Source of heading or term: kfmod | 1   
Source of heading or term: kktb | 3   
Source of heading or term: kktzm | 16   
Source of heading or term: lacc | 1   
Source of heading or term: lacgft | 1   
Source of heading or term: larpcal | 38   
Source of heading or term: larpcal. | 1   
Source of heading or term: lccgft | 1   
Source of heading or term: lcco | 28   
Source of heading or term: lcdgt | 42   
Source of heading or term: lcfgt | 6   
Source of heading or term: lcg | 19   
Source of heading or term: lcgf | 1   
Source of heading or term: lcgfft | 1   
Source of heading or term: lcgft | 14,798   
Source of heading or term: lcgft. | 194   
Source of heading or term: lcgft.?UNAUTHORIZED | 1   
Source of heading or term: lcgft?UNAUTHORIZED | 2   
Source of heading or term: lcgftUNAUTHORIZED | 1   
Source of heading or term: lcght | 2   
Source of heading or term: lcght. | 1   
Source of heading or term: lcgt | 2   
Source of heading or term: lcmpt | 1   
Source of heading or term: lcsfh | 1   
Source of heading or term: lcsh | 2,788   
Source of heading or term: lcsh. | 88   
Source of heading or term: lcshac | 5   
Source of heading or term: local | 7,182   
Source of heading or term: local. | 27   
Source of heading or term: marcgt | 32   
Source of heading or term: mesh | 6   
Source of heading or term: mesh. | 1   
Source of heading or term: migfg | 257   
Source of heading or term: mim | 7   
Source of heading or term: musician. | 1   
Source of heading or term: naf | 200   
Source of heading or term: narrator. | 3   
Source of heading or term: nasat | 1   
Source of heading or term: nc | 1   
Source of heading or term: nipo | 1   
Source of heading or term: njb | 7   
Source of heading or term: njb/9 | 7   
Source of heading or term: nli | 9   
Source of heading or term: olacvggt | 2   
Source of heading or term: optical | 1   
Source of heading or term: pda | 2   
Source of heading or term: pmbok | 6   
Source of heading or term: ppls | 9   
Source of heading or term: producer. | 2   
Source of heading or term: qlsp | 42   
Source of heading or term: r | 1   
Source of heading or term: radbs | 2   
Source of heading or term: radcarrier | 1   
Source of heading or term: ram | 64   
Source of heading or term: ram. | 3   
Source of heading or term: rasuqam | 5   
Source of heading or term: rbbin | 10   
Source of heading or term: rbgenr | 17   
Source of heading or term: rbprov | 1   
Source of heading or term: rbpub | 1   
Source of heading or term: rda | 3,256   
Source of heading or term: rda,edia | 1   
Source of heading or term: rda346 | 1   
Source of heading or term: rdaFT | 1   
Source of heading or term: rdaar | 2   
Source of heading or term: rdabs | 172   
Source of heading or term: rdacaontent | 1   
Source of heading or term: rdacarreir | 6   
Source of heading or term: rdacarrier | 36,363   
Source of heading or term: rdacarrier. | 1   
Source of heading or term: rdacarrier/dut | 10   
Source of heading or term: rdacarrier/fre | 1   
Source of heading or term: rdacarrier/ger | 2   
Source of heading or term: rdacarrier/swe | 1   
Source of heading or term: rdacarrier0+3 | 1   
Source of heading or term: rdacc | 4   
Source of heading or term: rdacont | 1   
Source of heading or term: rdaconten | 2   
Source of heading or term: rdacontent | 41,119   
Source of heading or term: rdacontent. | 1   
Source of heading or term: rdacontent/dut | 10   
Source of heading or term: rdacontent/fre | 2   
Source of heading or term: rdacontent/ger | 2   
Source of heading or term: rdacontent/spa | 2   
Source of heading or term: rdacontent/swe | 3   
Source of heading or term: rdacontenttext | 2   
Source of heading or term: rdaconyent | 1   
Source of heading or term: rdacpa | 2   
Source of heading or term: rdacpc | 258   
Source of heading or term: rdafs | 29   
Source of heading or term: rdaft | 351   
Source of heading or term: rdaill | 1   
Source of heading or term: rdamat | 42   
Source of heading or term: rdamedai | 1   
Source of heading or term: rdamedia | 36,650   
Source of heading or term: rdamedia. | 1   
Source of heading or term: rdamedia/dut | 10   
Source of heading or term: rdamedia/fre | 1   
Source of heading or term: rdamedia/ger | 2   
Source of heading or term: rdamedia/spa | 2   
Source of heading or term: rdamedia/swe | 2   
Source of heading or term: rdamedja | 1   
Source of heading or term: rdameida | 2   
Source of heading or term: rdanmedia | 1   
Source of heading or term: rdapc | 5   
Source of heading or term: rdapm | 10   
Source of heading or term: rdare | 184   
Source of heading or term: rdarft | 1   
Source of heading or term: rdarm | 276   
Source of heading or term: rdart | 3   
Source of heading or term: rdaspc | 2   
Source of heading or term: rdatr | 294   
Source of heading or term: rdatrm | 1   
Source of heading or term: rdatype | 1   
Source of heading or term: rdavolume | 1   
Source of heading or term: rdcaontent | 1   
Source of heading or term: rdcarrier | 13   
Source of heading or term: rdcontent | 2   
Source of heading or term: rdmedia | 6   
Source of heading or term: renib | 17   
Source of heading or term: rero | 2   
Source of heading or term: rvk | 23   
Source of heading or term: rvmgf | 88   
Source of heading or term: safd | 2   
Source of heading or term: sagfd | 1   
Source of heading or term: sao | 10   
Source of heading or term: saogf | 1   
Source of heading or term: sears | 2,263   
Source of heading or term: sears. | 18   
Source of heading or term: sgafd | 6   
Source of heading or term: sigle | 2   
Source of heading or term: ssgn | 1   
Source of heading or term: ssi | 3   
Source of heading or term: star | 2   
Source of heading or term: sti | 1   
Source of heading or term: still | 1   
Source of heading or term: stub | 2   
Source of heading or term: swd | 85   
Source of heading or term: tlcgt | 33   
Source of heading or term: tlctarget | 3   
Source of heading or term: ukmarc | 55   
Source of heading or term: ukslc | 10   
Source of heading or term: unbisn | 3   
Source of heading or term: unbist | 29   
Source of heading or term: undoc | 5   
Source of heading or term: undocs | 4   
Source of heading or term: unknown | 17   
Source of heading or term: unmediated | 1   
Source of heading or term: unsales | 1   
Source of heading or term: vgmsgg | 1   
Source of heading or term: vmj | 4   
Source of heading or term: wais | 15   
Source of heading or term: z | 8   
Source of heading or term: zdbs | 1   
</details>   
   
## Mapped note types    
Library action: **REVIEW** <br/>The created FOLIO records contain the following Note type values.  <br/>The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 47 things</summary>     
   
Measure | Count   
--- | ---:   
255 (Cartographic Mathematical Data) -> Cartographic Mathematical Data | 121   
500 (General note) -> General note | 103,230   
501 (With note) -> With note | 33   
502 (Dissertation note) -> Dissertation note | 54   
504 (Bibliography note) -> Bibliography note | 43,226   
505 (Formatted Contents Note) -> Formatted Contents Note | 25,728   
506 (Restrictions on Access note) -> Restrictions on Access note | 56   
507 (Scale note for graphic material) -> Scale note for graphic material | 1   
508 (Creation / Production Credits note) -> Creation / Production Credits note | 3,068   
510 (Citation / References note) -> Citation / References note | 225   
511 (Participant or Performer note) -> Participant or Performer note | 4,223   
513 (Type of report and period covered note) -> Type of report and period covered note | 2   
515 (Numbering peculiarities note) -> Numbering peculiarities note | 116   
516 (Type of computer file or data note) -> Type of computer file or data note | 5   
518 (Date / time and place of an event note) -> Date / time and place of an event note | 214   
520 (Summary) -> Summary | 66,361   
521 (Target Audience note) -> Target Audience note | 14,774   
522 (Geographic Coverage note) -> Geographic Coverage note | 1   
525 (Supplement note) -> Supplement note | 88   
526 (Study Program Information note) -> Study Program Information note | 1,581   
530 (Additional Physical Form Available note) -> Additional Physical Form Available note | 502   
533 (Reproduction note) -> Reproduction note | 2,120   
534 (Original Version note) -> Original Version note | 40   
535 (Location of Originals / Duplicates note) -> Location of Originals / Duplicates note | 2   
536 (Funding Information Note) -> Funding Information Note | 22   
538 (System Details note) -> System Details note | 6,815   
540 (Terms Governing Use and Reproduction note) -> Terms Governing Use and Reproduction note | 189   
541 (Immediate Source of Acquisition note) -> Immediate Source of Acquisition note | 17   
542 (Information related to Copyright Status) -> Information related to Copyright Status | 6   
544 (Location of Other Archival Materials note) -> Location of Other Archival Materials note | 1   
545 (Biographical or Historical Data) -> Biographical or Historical Data | 95   
546 (Language note) -> Language note | 3,752   
547 (Former Title Complexity note) -> Former Title Complexity note | 2   
550 (Issuing Body note) -> Issuing Body note | 115   
555 (Cumulative Index / Finding Aides notes) -> Cumulative Index / Finding Aides notes | 28   
556 (Information About Documentation note) -> Information About Documentation note | 1   
561 (Ownership and Custodial History note) -> Ownership and Custodial History note | 2   
562 (Copy and Version Identification note) -> Copy and Version Identification note | 2   
563 (Binding Information note) -> Binding Information note | 2   
580 (Linking Entry Complexity note) -> Linking Entry Complexity note | 84   
583 (Action note) -> Action note | 11   
586 (Awards note) -> Awards note | 1,376   
588 (Source of Description note) -> Source of Description note | 251   
880 (Formatted Contents Note) -> Formatted Contents Note | 2   
880 (General note) -> General note | 13   
880 (Summary) -> Summary | 2   
</details>   
   
## Mapped Alternative title types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Alternative title type values. The library should review the total number for each value against what they would expect to see mapped. The FOLIO community recommends a coarse-grained mapping.    
<details><summary>Click to expand all 4 things</summary>     
   
Measure | Count   
--- | ---:   
Former title | 4   
Uniform title | 5,423   
Variant title | 26,545   
</details>   
   
## Contributor type mapping    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Contributor type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 1214 things</summary>     
   
Measure | Count   
--- | ---:   
Contributor type code Actor found for $4 "act" (act)) | 1,026   
Contributor type code Actor found for $4 "act." (act)) | 71   
Contributor type code Adapter found for $4 "adp" (adp)) | 3   
Contributor type code Adapter found for $4 "adp." (adp)) | 3   
Contributor type code Animator found for $4 "anm" (anm)) | 7   
Contributor type code Arranger found for $4 "arr" (arr)) | 3   
Contributor type code Arranger found for $4 "arr." (arr)) | 8   
Contributor type code Artist found for $4 "art" (art)) | 2   
Contributor type code Artistic director found for $4 "ard" (ard)) | 10   
Contributor type code Author found for $4 "aut" (aut)) | 37   
Contributor type code Author found for $4 "aut." (aut)) | 5   
Contributor type code Author of afterword, colophon, etc. found for $4 "aft" (aft)) | 1   
Contributor type code Author of introduction, etc. found for $4 "aui" (aui)) | 3   
Contributor type code Bibliographic antecedent found for $4 "ant" (ant)) | 4   
Contributor type code Book designer found for $4 "bkd" (bkd)) | 19   
Contributor type code Book producer found for $4 "bkp" (bkp)) | 1   
Contributor type code Broadcaster found for $4 "brd" (brd)) | 1   
Contributor type code Cartographer found for $4 "ctg" (ctg)) | 1   
Contributor type code Choreographer found for $4 "chr" (chr)) | 1   
Contributor type code Choreographer found for $4 "chr." (chr)) | 1   
Contributor type code Cinematographer found for $4 "cng" (cng)) | 43   
Contributor type code Cinematographer found for $4 "cng." (cng)) | 1   
Contributor type code Collection registrar found for $4 "cor" (cor)) | 15   
Contributor type code Colorist found for $4 "clr" (clr)) | 3   
Contributor type code Compiler found for $4 "com" (com)) | 6   
Contributor type code Compiler found for $4 "com." (com)) | 2   
Contributor type code Composer found for $4 "cmp" (cmp)) | 80   
Contributor type code Composer found for $4 "cmp." (cmp)) | 7   
Contributor type code Conductor found for $4 "cnd." (cnd)) | 1   
Contributor type code Costume designer found for $4 "cst" (cst)) | 20   
Contributor type code Costume designer found for $4 "cst." (cst)) | 2   
Contributor type code Creator found for $4 "cre" (cre)) | 7   
Contributor type code Designer found for $4 "dsr" (dsr)) | 22   
Contributor type code Director found for $4 "drt" (drt)) | 111   
Contributor type code Director found for $4 "drt." (drt)) | 11   
Contributor type code Distributor found for $4 "dst" (dst)) | 2   
Contributor type code Donor found for $4 "dnr." (dnr)) | 1   
Contributor type code Editor found for $4 "edt" (edt)) | 51   
Contributor type code Editor found for $4 "edt." (edt)) | 3   
Contributor type code Film director found for $4 "fmd" (fmd)) | 1   
Contributor type code Film distributor found for $4 "fds" (fds)) | 1   
Contributor type code Film editor found for $4 "flm" (flm)) | 53   
Contributor type code Film editor found for $4 "flm." (flm)) | 2   
Contributor type code Film producer found for $4 "fmp" (fmp)) | 2   
Contributor type code Host found for $4 "hst" (hst)) | 4   
Contributor type code Host found for $4 "hst." (hst)) | 3   
Contributor type code Illustrator found for $4 "ill" (ill)) | 40   
Contributor type code Illustrator found for $4 "ill." (ill)) | 21   
Contributor type code Interviewee found for $4 "ive" (ive)) | 19   
Contributor type code Issuing body found for $4 "isb" (isb)) | 3   
Contributor type code Librettist found for $4 "lbt." (lbt)) | 2   
Contributor type code Lyricist found for $4 "lyr" (lyr)) | 1   
Contributor type code Lyricist found for $4 "lyr." (lyr)) | 1   
Contributor type code Narrator found for $4 "nrt" (nrt)) | 53   
Contributor type code Narrator found for $4 "nrt." (nrt)) | 128   
Contributor type code Other found for $4 "oth" (oth)) | 1   
Contributor type code Performer found for $4 "prf" (prf)) | 50   
Contributor type code Performer found for $4 "prf." (prf)) | 97   
Contributor type code Photographer found for $4 "pht" (pht)) | 7   
Contributor type code Photographer found for $4 "pht." (pht)) | 1   
Contributor type code Printer found for $4 "prt" (prt)) | 2   
Contributor type code Producer found for $4 "pro" (pro)) | 390   
Contributor type code Producer found for $4 "pro." (pro)) | 24   
Contributor type code Production company found for $4 "prn" (prn)) | 4   
Contributor type code Production manager found for $4 "pmn" (pmn)) | 3   
Contributor type code Production personnel found for $4 "prd" (prd)) | 14   
Contributor type code Production personnel found for $4 "prd." (prd)) | 1   
Contributor type code Publisher found for $4 "pbl" (pbl)) | 38   
Contributor type code Reporter found for $4 "rpt" (rpt)) | 2   
Contributor type code Screenwriter found for $4 "aus" (aus)) | 194   
Contributor type code Screenwriter found for $4 "aus." (aus)) | 11   
Contributor type code Set designer found for $4 "std" (std)) | 1   
Contributor type code Set designer found for $4 "std." (std)) | 1   
Contributor type code Singer found for $4 "sng" (sng)) | 1   
Contributor type code Transcriber found for $4 "trc" (trc)) | 2   
Contributor type code Transcriber found for $4 "trc." (trc)) | 1   
Contributor type code Translator found for $4 "trl" (trl)) | 17   
Contributor type code Translator found for $4 "trl." (trl)) | 9   
Contributor type name Abridger found for 100 $e abridger (abridger.)  | 1   
Contributor type name Abridger found for 700 $e abridger (abridger)  | 1   
Contributor type name Abridger found for 700 $e abridger (abridger.)  | 119   
Contributor type name Actor found for 700 $e actor (actor)  | 150   
Contributor type name Actor found for 700 $e actor (actor,)  | 8   
Contributor type name Actor found for 700 $e actor (actor.)  | 2,285   
Contributor type name Adapter found for 100 $e adapter (adapter)  | 2   
Contributor type name Adapter found for 100 $e adapter (adapter.)  | 40   
Contributor type name Adapter found for 700 $e adapter (adapter,)  | 5   
Contributor type name Adapter found for 700 $e adapter (adapter.)  | 92   
Contributor type name Adapter found for 710 $e adapter (adapter.)  | 1   
Contributor type name Animator found for 700 $e animator (animator,)  | 3   
Contributor type name Animator found for 700 $e animator (animator.)  | 15   
Contributor type name Animator found for 710 $e animator (animator.)  | 3   
Contributor type name Arranger found for 700 $e arranger (arranger)  | 2   
Contributor type name Arranger found for 700 $e arranger (arranger.)  | 7   
Contributor type name Art director found for 700 $e art director (art director)  | 4   
Contributor type name Art director found for 700 $e art director (art director.)  | 9   
Contributor type name Artist found for 100 $e artist (artist)  | 1   
Contributor type name Artist found for 100 $e artist (artist,)  | 14   
Contributor type name Artist found for 100 $e artist (artist.)  | 8   
Contributor type name Artist found for 700 $e artist (artist)  | 85   
Contributor type name Artist found for 700 $e artist (artist,)  | 32   
Contributor type name Artist found for 700 $e artist (artist.)  | 532   
Contributor type name Artist found for 700 $e artist (artist.-)  | 1   
Contributor type name Artist found for 710 $e artist (artist)  | 1   
Contributor type name Artist found for 710 $e artist (artist.)  | 3   
Contributor type name Artistic director found for 700 $e artistic director (artistic director.)  | 2   
Contributor type name Author found for 100 $e Author (Author.)  | 2   
Contributor type name Author found for 100 $e author ( author.)  | 7   
Contributor type name Author found for 100 $e author (author)  | 633   
Contributor type name Author found for 100 $e author (author, )  | 28   
Contributor type name Author found for 100 $e author (author,)  | 639   
Contributor type name Author found for 100 $e author (author.                                                             )  | 1   
Contributor type name Author found for 100 $e author (author.                           )  | 1   
Contributor type name Author found for 100 $e author (author.  )  | 1   
Contributor type name Author found for 100 $e author (author. )  | 24   
Contributor type name Author found for 100 $e author (author.)  | 15,146   
Contributor type name Author found for 100 $e author (author..)  | 1   
Contributor type name Author found for 110 $e author (author)  | 2   
Contributor type name Author found for 110 $e author (author,)  | 4   
Contributor type name Author found for 110 $e author (author.)  | 27   
Contributor type name Author found for 111 $j author (author.)  | 4   
Contributor type name Author found for 700 $e author ( author.)  | 2   
Contributor type name Author found for 700 $e author (author)  | 206   
Contributor type name Author found for 700 $e author (author, )  | 3   
Contributor type name Author found for 700 $e author (author,)  | 65   
Contributor type name Author found for 700 $e author (author,.)  | 1   
Contributor type name Author found for 700 $e author (author. )  | 5   
Contributor type name Author found for 700 $e author (author.)  | 2,518   
Contributor type name Author found for 700 $e author (author..)  | 2   
Contributor type name Author found for 710 $e author (author)  | 1   
Contributor type name Author found for 710 $e author (author,)  | 2   
Contributor type name Author found for 710 $e author (author.)  | 28   
Contributor type name Book designer found for 700 $e book designer (book designer)  | 5   
Contributor type name Book designer found for 700 $e book designer (book designer.)  | 21   
Contributor type name Book designer found for 710 $e book designer (book designer.)  | 2   
Contributor type name Book producer found for 110 $e book producer (book producer.)  | 1   
Contributor type name Bookjacket designer found for 700 $e bookjacket designer (bookjacket designer,)  | 1   
Contributor type name Bookjacket designer found for 700 $e bookjacket designer (bookjacket designer.)  | 1   
Contributor type name Broadcaster found for 710 $e broadcaster (broadcaster.)  | 13   
Contributor type name Cartographer found for 700 $e cartographer (cartographer,)  | 1   
Contributor type name Choreographer found for 700 $e choreographer (choreographer.)  | 4   
Contributor type name Cinematographer found for 700 $e cinematographer (cinematographer)  | 5   
Contributor type name Cinematographer found for 700 $e cinematographer (cinematographer.)  | 62   
Contributor type name Collector found for 700 $e collector (collector.)  | 1   
Contributor type name Colorist found for 700 $e colorist (colorist)  | 8   
Contributor type name Colorist found for 700 $e colorist (colorist,)  | 1   
Contributor type name Colorist found for 700 $e colorist (colorist.)  | 146   
Contributor type name Colorist found for 710 $e colorist (colorist.)  | 2   
Contributor type name Commentator found for 700 $e commentator (commentator,)  | 1   
Contributor type name Commentator found for 700 $e commentator (commentator.)  | 5   
Contributor type name Compiler found for 100 $e compiler (compiler)  | 2   
Contributor type name Compiler found for 100 $e compiler (compiler.)  | 17   
Contributor type name Compiler found for 110 $e compiler (compiler.)  | 2   
Contributor type name Compiler found for 700 $e compiler ( compiler.)  | 1   
Contributor type name Compiler found for 700 $e compiler (compiler)  | 7   
Contributor type name Compiler found for 700 $e compiler (compiler,)  | 6   
Contributor type name Compiler found for 700 $e compiler (compiler.)  | 140   
Contributor type name Composer found for 100 $e composer (composer)  | 1   
Contributor type name Composer found for 100 $e composer (composer,)  | 2   
Contributor type name Composer found for 100 $e composer (composer.)  | 7   
Contributor type name Composer found for 700 $e composer (composer)  | 6   
Contributor type name Composer found for 700 $e composer (composer,)  | 6   
Contributor type name Composer found for 700 $e composer (composer.)  | 96   
Contributor type name Composer found for 710 $e composer (composer.)  | 1   
Contributor type name Conceptor found for 700 $e conceptor (conceptor.)  | 2   
Contributor type name Conductor found for 700 $e conductor (conductor)  | 1   
Contributor type name Conductor found for 700 $e conductor (conductor,)  | 1   
Contributor type name Conductor found for 700 $e conductor (conductor.)  | 1   
Contributor type name Consultant found for 700 $e consultant (consultant.)  | 54   
Contributor type name Contributor found for 100 $e contributor (contributor.)  | 1   
Contributor type name Contributor found for 700 $e contributor (contributor)  | 13   
Contributor type name Contributor found for 700 $e contributor (contributor.)  | 233   
Contributor type name Contributor found for 710 $e contributor (contributor.)  | 9   
Contributor type name Copyright holder found for 710 $e copyright holder (copyright holder.)  | 4   
Contributor type name Costume designer found for 700 $e costume designer (costume designer)  | 5   
Contributor type name Costume designer found for 700 $e costume designer (costume designer.)  | 69   
Contributor type name Cover designer found for 700 $e cover designer (cover designer,)  | 1   
Contributor type name Cover designer found for 700 $e cover designer (cover designer.)  | 8   
Contributor type name Creator found for 100 $e creator ([creator].)  | 1   
Contributor type name Creator found for 100 $e creator (creator)  | 1   
Contributor type name Creator found for 100 $e creator (creator, )  | 7   
Contributor type name Creator found for 100 $e creator (creator,)  | 4   
Contributor type name Creator found for 100 $e creator (creator.)  | 3   
Contributor type name Creator found for 700 $e creator (creator )  | 3   
Contributor type name Creator found for 700 $e creator (creator)  | 10   
Contributor type name Creator found for 700 $e creator (creator,)  | 18   
Contributor type name Creator found for 700 $e creator (creator.)  | 186   
Contributor type name Creator found for 710 $e creator (creator.)  | 1   
Contributor type name Curator found for 100 $e curator (curator)  | 1   
Contributor type name Curator found for 700 $e curator (curator.)  | 2   
Contributor type name Designer found for 100 $e designer (designer)  | 1   
Contributor type name Designer found for 700 $e designer (designer)  | 1   
Contributor type name Designer found for 700 $e designer (designer,)  | 1   
Contributor type name Designer found for 700 $e designer (designer.)  | 147   
Contributor type name Director found for 700 $e Director (Director.)  | 3   
Contributor type name Director found for 700 $e director (director )  | 3   
Contributor type name Director found for 700 $e director (director)  | 29   
Contributor type name Director found for 700 $e director (director, )  | 1   
Contributor type name Director found for 700 $e director (director,)  | 57   
Contributor type name Director found for 700 $e director (director.)  | 1,014   
Contributor type name Director found for 710 $e director (director,)  | 1   
Contributor type name Director found for 710 $e director (director.)  | 6   
Contributor type name Distributor found for 710 $e distributor (distributor)  | 1   
Contributor type name Distributor found for 710 $e distributor (distributor.)  | 37   
Contributor type name Donor found for 700 $e donor (donor.)  | 3   
Contributor type name Editor found for 100 $e editor (editor.)  | 8   
Contributor type name Editor found for 700 $e Editor (Editor)  | 2   
Contributor type name Editor found for 700 $e Editor (Editor.)  | 7   
Contributor type name Editor found for 700 $e editor ( editor.)  | 1   
Contributor type name Editor found for 700 $e editor ([editor].)  | 1   
Contributor type name Editor found for 700 $e editor (editor)  | 84   
Contributor type name Editor found for 700 $e editor (editor, )  | 2   
Contributor type name Editor found for 700 $e editor (editor,)  | 50   
Contributor type name Editor found for 700 $e editor (editor.)  | 1,256   
Contributor type name Editor found for 710 $e editor (editor)  | 2   
Contributor type name Editor found for 710 $e editor (editor.)  | 21   
Contributor type name Editor of compilation found for 700 $e editor of compilation (editor of compilation)  | 17   
Contributor type name Editor of compilation found for 700 $e editor of compilation (editor of compilation,)  | 3   
Contributor type name Editor of compilation found for 700 $e editor of compilation (editor of compilation.)  | 58   
Contributor type name Editor of moving image work found for 700 $e editor of moving image work (editor of moving image work)  | 12   
Contributor type name Editor of moving image work found for 700 $e editor of moving image work (editor of moving image work,)  | 2   
Contributor type name Editor of moving image work found for 700 $e editor of moving image work (editor of moving image work.)  | 100   
Contributor type name Engineer found for 700 $e engineer (engineer)  | 1   
Contributor type name Engineer found for 700 $e engineer (engineer.)  | 1   
Contributor type name Film director found for 700 $e film director (film director)  | 8   
Contributor type name Film director found for 700 $e film director (film director,)  | 86   
Contributor type name Film director found for 700 $e film director (film director.)  | 143   
Contributor type name Film distributor found for 710 $e film distributor (film distributor)  | 1   
Contributor type name Film distributor found for 710 $e film distributor (film distributor,)  | 1   
Contributor type name Film distributor found for 710 $e film distributor (film distributor.)  | 174   
Contributor type name Film editor found for 700 $e film editor (film editor)  | 4   
Contributor type name Film editor found for 700 $e film editor (film editor,)  | 2   
Contributor type name Film editor found for 700 $e film editor (film editor.)  | 60   
Contributor type name Film producer found for 700 $e film producer (film producer)  | 37   
Contributor type name Film producer found for 700 $e film producer (film producer,)  | 47   
Contributor type name Film producer found for 700 $e film producer (film producer.)  | 544   
Contributor type name Film producer found for 710 $e film producer (film producer.)  | 6   
Contributor type name Filmmaker found for 700 $e filmmaker (filmmaker.)  | 4   
Contributor type name Former owner found for 700 $e former owner (former owner.)  | 1   
Contributor type name Funder found for 710 $e funder (funder.)  | 3   
Contributor type name Host found for 100 $e host (host.)  | 1   
Contributor type name Host found for 700 $e host (host)  | 1   
Contributor type name Host found for 700 $e host (host.)  | 4   
Contributor type name Host institution found for 710 $e host institution (host institution)  | 2   
Contributor type name Host institution found for 710 $e host institution (host institution,)  | 2   
Contributor type name Host institution found for 710 $e host institution (host institution.)  | 5   
Contributor type name Illustrator found for 100 $e illustrator (illustrator,)  | 3   
Contributor type name Illustrator found for 100 $e illustrator (illustrator.)  | 47   
Contributor type name Illustrator found for 700 $e Illustrator (Illustrator)  | 1   
Contributor type name Illustrator found for 700 $e Illustrator (Illustrator.)  | 1   
Contributor type name Illustrator found for 700 $e illustrator ( illustrator.)  | 2   
Contributor type name Illustrator found for 700 $e illustrator ([illustrator])  | 7   
Contributor type name Illustrator found for 700 $e illustrator (illustrator )  | 1   
Contributor type name Illustrator found for 700 $e illustrator (illustrator)  | 192   
Contributor type name Illustrator found for 700 $e illustrator (illustrator,)  | 7   
Contributor type name Illustrator found for 700 $e illustrator (illustrator.)  | 4,419   
Contributor type name Illustrator found for 700 $e illustrator (illustrator..)  | 1   
Contributor type name Illustrator found for 710 $e illustrator (illustrator)  | 3   
Contributor type name Illustrator found for 710 $e illustrator (illustrator.)  | 61   
Contributor type name Instrumentalist found for 700 $e instrumentalist (instrumentalist.)  | 4   
Contributor type name Interviewee found for 700 $e interviewee (interviewee,)  | 5   
Contributor type name Interviewee found for 700 $e interviewee (interviewee.)  | 89   
Contributor type name Interviewer found for 700 $e interviewer (interviewer)  | 1   
Contributor type name Interviewer found for 700 $e interviewer (interviewer.)  | 3   
Contributor type name Issuing body found for 110 $e issuing body (issuing body.)  | 15   
Contributor type name Issuing body found for 710 $e issuing body (issuing body,)  | 4   
Contributor type name Issuing body found for 710 $e issuing body (issuing body.)  | 65   
Contributor type name Issuing body found for 711 $j issuing body (issuing body)  | 1   
Contributor type name Issuing body found for 720 $e issuing body (issuing body.)  | 9   
Contributor type name Lyricist found for 700 $e lyricist (lyricist.)  | 8   
Contributor type name Manufacturer found for 710 $e manufacturer (manufacturer)  | 2   
Contributor type name Manufacturer found for 710 $e manufacturer (manufacturer.)  | 8   
Contributor type name Musical director found for 700 $e musical director (musical director.)  | 2   
Contributor type name Musician found for 100 $e Musician ((Musician))  | 1   
Contributor type name Musician found for 100 $e musician ((musician))  | 7   
Contributor type name Musician found for 100 $e musician (musician.)  | 4   
Contributor type name Musician found for 700 $e Musician ((Musician))  | 1   
Contributor type name Musician found for 700 $e musician ((musician))  | 6   
Contributor type name Musician found for 700 $e musician (musician)  | 2   
Contributor type name Musician found for 700 $e musician (musician.)  | 49   
Contributor type name Narrator found for 100 $e narrator (narrator.)  | 6   
Contributor type name Narrator found for 700 $e Narrator (Narrator.)  | 1   
Contributor type name Narrator found for 700 $e narrator ([narrator].)  | 1   
Contributor type name Narrator found for 700 $e narrator (narrator)  | 30   
Contributor type name Narrator found for 700 $e narrator (narrator,)  | 9   
Contributor type name Narrator found for 700 $e narrator (narrator.)  | 1,626   
Contributor type name Papermaker found for 700 $e papermaker (papermaker.)  | 2   
Contributor type name Performer found for 100 $e performer (performer. )  | 4   
Contributor type name Performer found for 100 $e performer (performer.  )  | 1   
Contributor type name Performer found for 100 $e performer (performer.)  | 37   
Contributor type name Performer found for 700 $e performer ((performer).)  | 1   
Contributor type name Performer found for 700 $e performer (performer)  | 3   
Contributor type name Performer found for 700 $e performer (performer,)  | 6   
Contributor type name Performer found for 700 $e performer (performer.)  | 166   
Contributor type name Performer found for 710 $e performer (performer.)  | 2   
Contributor type name Photographer found for 100 $e photographer (photographer,)  | 1   
Contributor type name Photographer found for 100 $e photographer (photographer.)  | 6   
Contributor type name Photographer found for 700 $e photographer (photographer)  | 4   
Contributor type name Photographer found for 700 $e photographer (photographer.)  | 129   
Contributor type name Presenter found for 700 $e presenter (presenter,)  | 1   
Contributor type name Presenter found for 700 $e presenter (presenter.)  | 3   
Contributor type name Presenter found for 710 $e presenter (presenter)  | 7   
Contributor type name Presenter found for 710 $e presenter (presenter,)  | 34   
Contributor type name Presenter found for 710 $e presenter (presenter.)  | 127   
Contributor type name Printer found for 710 $e printer (printer.)  | 8   
Contributor type name Printmaker found for 700 $e printmaker (printmaker,)  | 1   
Contributor type name Printmaker found for 700 $e printmaker (printmaker.)  | 2   
Contributor type name Producer found for 100 $e producer (producer.)  | 1   
Contributor type name Producer found for 700 $e Producer (Producer.)  | 5   
Contributor type name Producer found for 700 $e producer (producer )  | 3   
Contributor type name Producer found for 700 $e producer (producer)  | 33   
Contributor type name Producer found for 700 $e producer (producer, )  | 4   
Contributor type name Producer found for 700 $e producer (producer,)  | 93   
Contributor type name Producer found for 700 $e producer (producer.)  | 690   
Contributor type name Producer found for 710 $e Producer (Producer.)  | 1   
Contributor type name Producer found for 710 $e producer (producer,)  | 1   
Contributor type name Producer found for 710 $e producer (producer.)  | 35   
Contributor type name Production company found for 710 $e production company (production company)  | 7   
Contributor type name Production company found for 710 $e production company (production company,)  | 27   
Contributor type name Production company found for 710 $e production company (production company.)  | 602   
Contributor type name Production designer found for 700 $e production designer (production designer)  | 6   
Contributor type name Production designer found for 700 $e production designer (production designer,)  | 1   
Contributor type name Production designer found for 700 $e production designer (production designer.)  | 71   
Contributor type name Production manager found for 700 $e production manager (production manager.)  | 1   
Contributor type name Programmer found for 700 $e programmer (programmer.)  | 2   
Contributor type name Project director found for 700 $e project director (project director)  | 1   
Contributor type name Project director found for 700 $e project director (project director.)  | 1   
Contributor type name Publisher found for 700 $e publisher (publisher)  | 1   
Contributor type name Publisher found for 700 $e publisher (publisher,)  | 2   
Contributor type name Publisher found for 700 $e publisher (publisher.)  | 10   
Contributor type name Publisher found for 710 $e publisher (publisher)  | 4   
Contributor type name Publisher found for 710 $e publisher (publisher,)  | 6   
Contributor type name Publisher found for 710 $e publisher (publisher.)  | 228   
Contributor type name Publisher found for 710 $e publisher (publisher.))  | 1   
Contributor type name Publisher found for 720 $e publisher (publisher.)  | 3   
Contributor type name Recording engineer found for 700 $e recording engineer (recording engineer.)  | 1   
Contributor type name Reporter found for 700 $e reporter (reporter,)  | 1   
Contributor type name Researcher found for 100 $e researcher (researcher,)  | 1   
Contributor type name Researcher found for 700 $e researcher (researcher,)  | 2   
Contributor type name Researcher found for 700 $e researcher (researcher.)  | 13   
Contributor type name Reviewer found for 700 $e reviewer (reviewer.)  | 1   
Contributor type name Screenwriter found for 700 $e screenwriter (screenwriter)  | 20   
Contributor type name Screenwriter found for 700 $e screenwriter (screenwriter, )  | 5   
Contributor type name Screenwriter found for 700 $e screenwriter (screenwriter,)  | 81   
Contributor type name Screenwriter found for 700 $e screenwriter (screenwriter.)  | 353   
Contributor type name Sculptor found for 700 $e sculptor (sculptor.)  | 2   
Contributor type name Singer found for 100 $e singer (singer.)  | 2   
Contributor type name Singer found for 700 $e singer (singer.)  | 18   
Contributor type name Sponsor found for 710 $e sponsor (sponsor.)  | 3   
Contributor type name Storyteller found for 700 $e storyteller (storyteller.)  | 11   
Contributor type name Teacher found for 700 $e teacher (teacher.)  | 2   
Contributor type name Television director found for 700 $e television director (television director)  | 1   
Contributor type name Television director found for 700 $e television director (television director.)  | 38   
Contributor type name Television producer found for 700 $e television producer (television producer)  | 2   
Contributor type name Television producer found for 700 $e television producer (television producer,)  | 18   
Contributor type name Television producer found for 700 $e television producer (television producer.)  | 34   
Contributor type name Translator found for 100 $e translator (translator,)  | 1   
Contributor type name Translator found for 100 $e translator (translator.)  | 1   
Contributor type name Translator found for 700 $e Translator ((Translator))  | 2   
Contributor type name Translator found for 700 $e Translator (Translator.)  | 4   
Contributor type name Translator found for 700 $e translator (translator)  | 20   
Contributor type name Translator found for 700 $e translator (translator,)  | 24   
Contributor type name Translator found for 700 $e translator (translator.)  | 551   
Contributor type name Translator found for 710 $e translator (translator.)  | 3   
Contributor type name Videographer found for 700 $e videographer (videographer.)  | 4   
Contributor type name Voice actor found for 700 $e voice actor (voice actor)  | 36   
Contributor type name Voice actor found for 700 $e voice actor (voice actor,)  | 6   
Contributor type name Voice actor found for 700 $e voice actor (voice actor.)  | 498   
Contributor type name Voice actor found for 710 $e voice actor (voice actor,)  | 1   
Contributor type name Writer of added commentary found for 700 $e writer of added commentary (writer of added commentary,)  | 1   
Contributor type name Writer of added commentary found for 700 $e writer of added commentary (writer of added commentary.)  | 3   
Contributor type name Writer of added text found for 700 $e writer of added text (writer of added text.)  | 2   
Contributor type name Writer of introduction found for 700 $e writer of introduction (writer of introduction)  | 2   
Contributor type name Writer of introduction found for 700 $e writer of introduction (writer of introduction,)  | 1   
Contributor type name Writer of introduction found for 700 $e writer of introduction (writer of introduction.)  | 72   
Contributor type name Writer of preface found for 700 $e writer of preface (writer of preface)  | 1   
Contributor type name Writer of preface found for 700 $e writer of preface (writer of preface.)  | 5   
Contributor type name Writer of supplementary textual content found for 700 $e writer of supplementary textual content (writer of supplementary textual content.)  | 9   
Mapping failed for $4 "author" (author)  | 2   
Mapping failed for $4 "dir." (dir)  | 1   
Mapping failed for $4 "ed." (ed)  | 7   
Mapping failed for $4 "editor" (editor)  | 1   
Mapping failed for $4 "editors" (editors)  | 3   
Mapping failed for $4 "ill.Z" (illZ)  | 1   
Mapping failed for $4 "illustrator" (illustrator)  | 4   
Mapping failed for $4 "illustrator." (illustrator)  | 10   
Mapping failed for $4 "illustrator.?UNAUTHORIZED" (illustratorUNAUTHORIZED)  | 1   
Mapping failed for $4 "ilt" (ilt)  | 12   
Mapping failed for $4 "jt. aut." (jt aut)  | 6   
Mapping failed for $4 "narrator." (narrator)  | 1   
Mapping failed for $4 "tr." (tr)  | 1   
Mapping failed for $4 "voc." (voc)  | 2   
Mapping failed for 100 $e  (Normalized: )  | 2   
Mapping failed for 100 $e (Calpyso singer) (Normalized: Calpyso singer)  | 2   
Mapping failed for 100 $e (Calypso Singer) (Normalized: Calypso Singer)  | 3   
Mapping failed for 100 $e (Calypso singer) (Normalized: Calypso singer)  | 16   
Mapping failed for 100 $e (calypso singer) (Normalized: calypso singer)  | 1   
Mapping failed for 100 $e (music band) (Normalized: music band)  | 1   
Mapping failed for 100 $e 1785-1863 (Normalized: 17851863)  | 1   
Mapping failed for 100 $e 1916-1990. (Normalized: 19161990)  | 1   
Mapping failed for 100 $e 1943- (Normalized: 1943)  | 2   
Mapping failed for 100 $e 1945- (Normalized: 1945)  | 1   
Mapping failed for 100 $e Embajador de Venezuela. (Normalized: Embajador de Venezuela)  | 1   
Mapping failed for 100 $e I, (Normalized: I)  | 1   
Mapping failed for 100 $e Minister of Mines and Forest. (Normalized: Minister of Mines and Forest)  | 1   
Mapping failed for 100 $e adaptor (Normalized: adaptor)  | 1   
Mapping failed for 100 $e adaptor. (Normalized: adaptor)  | 9   
Mapping failed for 100 $e aduthor. (Normalized: aduthor)  | 1   
Mapping failed for 100 $e athor. (Normalized: athor)  | 1   
Mapping failed for 100 $e atuhor. (Normalized: atuhor)  | 1   
Mapping failed for 100 $e auathor (Normalized: auathor)  | 1   
Mapping failed for 100 $e auhor. (Normalized: auhor)  | 1   
Mapping failed for 100 $e auhtor. (Normalized: auhtor)  | 1   
Mapping failed for 100 $e aurthor. (Normalized: aurthor)  | 1   
Mapping failed for 100 $e auteur (Normalized: auteur)  | 2   
Mapping failed for 100 $e auteur. (Normalized: auteur)  | 1   
Mapping failed for 100 $e author . (Normalized: author )  | 1   
Mapping failed for 100 $e author ; (Normalized: author )  | 1   
Mapping failed for 100 $e author ; illustrated by Anne Kennedy. (Normalized: author  illustrated by Anne Kennedy)  | 1   
Mapping failed for 100 $e author and illustrator (Normalized: author and illustrator)  | 1   
Mapping failed for 100 $e author, illustrator. (Normalized: author illustrator)  | 1   
Mapping failed for 100 $e author.246 (Normalized: author246)  | 1   
Mapping failed for 100 $e author.?UNAUTHORIZED (Normalized: authorUNAUTHORIZED)  | 4   
Mapping failed for 100 $e author.D (Normalized: authorD)  | 1   
Mapping failed for 100 $e author?UNAUTHORIZED (Normalized: authorUNAUTHORIZED)  | 2   
Mapping failed for 100 $e authour. (Normalized: authour)  | 3   
Mapping failed for 100 $e autor. (Normalized: autor)  | 3   
Mapping failed for 100 $e comp. (Normalized: comp)  | 83   
Mapping failed for 100 $e composer and arranger. (Normalized: composer and arranger)  | 1   
Mapping failed for 100 $e ed. (Normalized: ed)  | 78   
Mapping failed for 100 $e ed. and tr. (Normalized: ed and tr)  | 1   
Mapping failed for 100 $e editer. (Normalized: editer)  | 1   
Mapping failed for 100 $e executive producer, (Normalized: executive producer)  | 1   
Mapping failed for 100 $e ill. (Normalized: ill)  | 4   
Mapping failed for 100 $e illus. (Normalized: illus)  | 1   
Mapping failed for 100 $e music conductor. (Normalized: music conductor)  | 1   
Mapping failed for 100 $e perofrmer. (Normalized: perofrmer)  | 1   
Mapping failed for 100 $e photogapher, (Normalized: photogapher)  | 1   
Mapping failed for 100 $e playwright,  (Normalized: playwright)  | 2   
Mapping failed for 100 $e poet,  (Normalized: poet)  | 2   
Mapping failed for 100 $e pseud. (Normalized: pseud)  | 1   
Mapping failed for 100 $e tr. (Normalized: tr)  | 1   
Mapping failed for 100 $e uathor (Normalized: uathor)  | 1   
Mapping failed for 100 $e uathor. (Normalized: uathor)  | 1   
Mapping failed for 100 $e uthor. (Normalized: uthor)  | 1   
Mapping failed for 100 $e writer (Normalized: writer)  | 6   
Mapping failed for 100 $e writer, (Normalized: writer)  | 1   
Mapping failed for 100 $e writer. (Normalized: writer)  | 10   
Mapping failed for 110 $e (Music Band) (Normalized: Music Band)  | 1   
Mapping failed for 110 $e (Music band) (Normalized: Music band)  | 1   
Mapping failed for 110 $e (music band) (Normalized: music band)  | 4   
Mapping failed for 110 $e (musical group) (Normalized: musical group)  | 6   
Mapping failed for 110 $e Musical group (Normalized: Musical group)  | 2   
Mapping failed for 110 $e comp. (Normalized: comp)  | 1   
Mapping failed for 110 $e musical group. (Normalized: musical group)  | 1   
Mapping failed for 700 $e  (Normalized: )  | 6   
Mapping failed for 700 $e  design asst. (Normalized: design asst)  | 1   
Mapping failed for 700 $e  ed. (Normalized: ed)  | 14   
Mapping failed for 700 $e  ed.,intro. (Normalized: edintro)  | 1   
Mapping failed for 700 $e  editor-in-chief (Normalized: editorinchief)  | 1   
Mapping failed for 700 $e  editor-in-chief. (Normalized: editorinchief)  | 1   
Mapping failed for 700 $e  ill. (Normalized: ill)  | 33   
Mapping failed for 700 $e  joint author. (Normalized: joint author)  | 1   
Mapping failed for 700 $e  jt au. (Normalized: jt au)  | 3   
Mapping failed for 700 $e  jt. au. (Normalized: jt au)  | 1   
Mapping failed for 700 $e  jt. aut. (Normalized: jt aut)  | 4   
Mapping failed for 700 $e  jt. ed. (Normalized: jt ed)  | 1   
Mapping failed for 700 $e  jt.au. (Normalized: jtau)  | 1   
Mapping failed for 700 $e  jt.ed. (Normalized: jted)  | 1   
Mapping failed for 700 $e  pht. (Normalized: pht)  | 2   
Mapping failed for 700 $e  trans. (Normalized: trans)  | 1   
Mapping failed for 700 $e  writer of foreword. (Normalized: writer of foreword)  | 1   
Mapping failed for 700 $e "Butlerite" (Normalized: Butlerite)  | 4   
Mapping failed for 700 $e (Calypso Singer) (Normalized: Calypso Singer)  | 3   
Mapping failed for 700 $e (Calypso singer) (Normalized: Calypso singer)  | 22   
Mapping failed for 700 $e (calypso singer) (Normalized: calypso singer)  | 1   
Mapping failed for 700 $e ,ill. (Normalized: ill)  | 1   
Mapping failed for 700 $e ,jt. autr. (Normalized: jt autr)  | 1   
Mapping failed for 700 $e . (Normalized: )  | 2   
Mapping failed for 700 $e . aut. (Normalized:  aut)  | 1   
Mapping failed for 700 $e . editor. (Normalized:  editor)  | 1   
Mapping failed for 700 $e .ill. (Normalized: ill)  | 1   
Mapping failed for 700 $e 1785-1863 (Normalized: 17851863)  | 1   
Mapping failed for 700 $e 1786-1859 (Normalized: 17861859)  | 2   
Mapping failed for 700 $e 1923- (Normalized: 1923)  | 1   
Mapping failed for 700 $e 1ll. (Normalized: 1ll)  | 2   
Mapping failed for 700 $e Adaptation. (Normalized: Adaptation)  | 1   
Mapping failed for 700 $e Assistant Editor. (Normalized: Assistant Editor)  | 1   
Mapping failed for 700 $e Building adviser. (Normalized: Building adviser)  | 1   
Mapping failed for 700 $e Caribbean ed. (Normalized: Caribbean ed)  | 1   
Mapping failed for 700 $e Chairman, Dir./Town & Country Planning. (Normalized: Chairman DirTown  Country Planning)  | 1   
Mapping failed for 700 $e Chairman. (Normalized: Chairman)  | 15   
Mapping failed for 700 $e Comp. (Normalized: Comp)  | 3   
Mapping failed for 700 $e Content Editor (Normalized: Content Editor)  | 1   
Mapping failed for 700 $e Deno Caruana. (Normalized: Deno Caruana)  | 1   
Mapping failed for 700 $e Deputy Chairman. (Normalized: Deputy Chairman)  | 1   
Mapping failed for 700 $e Design. (Normalized: Design)  | 1   
Mapping failed for 700 $e Director of Research. (Normalized: Director of Research)  | 1   
Mapping failed for 700 $e ED. (Normalized: ED)  | 1   
Mapping failed for 700 $e Ed. (Normalized: Ed)  | 1   
Mapping failed for 700 $e Editor-in-Chief. (Normalized: EditorinChief)  | 1   
Mapping failed for 700 $e Executive Producer. (Normalized: Executive Producer)  | 22   
Mapping failed for 700 $e Executive producer. (Normalized: Executive producer)  | 1   
Mapping failed for 700 $e Éditeur scientifique. (Normalized: Editeur scientifique)  | 2   
Mapping failed for 700 $e Founder and Chairman. (Normalized: Founder and Chairman)  | 1   
Mapping failed for 700 $e Ill. (Normalized: Ill)  | 4   
Mapping failed for 700 $e Illus. (Normalized: Illus)  | 1   
Mapping failed for 700 $e John Patience,ill. (Normalized: John Patienceill)  | 1   
Mapping failed for 700 $e Joint author. (Normalized: Joint author)  | 1   
Mapping failed for 700 $e Jt. aut. (Normalized: Jt aut)  | 6   
Mapping failed for 700 $e Jt. auth. (Normalized: Jt auth)  | 1   
Mapping failed for 700 $e Jt.aut. (Normalized: Jtaut)  | 3   
Mapping failed for 700 $e Librarian. (Normalized: Librarian)  | 1   
Mapping failed for 700 $e Lindsay Duff, ill. (Normalized: Lindsay Duff ill)  | 1   
Mapping failed for 700 $e Lorrie Szekat.ill. (Normalized: Lorrie Szekatill)  | 1   
Mapping failed for 700 $e Master of Ceremonies. (Normalized: Master of Ceremonies)  | 1   
Mapping failed for 700 $e Ombudsman of Trinidad and Tobago (Normalized: Ombudsman of Trinidad and Tobago)  | 1   
Mapping failed for 700 $e Peter & Mary Speed. (Normalized: Peter  Mary Speed)  | 2   
Mapping failed for 700 $e Project leader. (Normalized: Project leader)  | 2   
Mapping failed for 700 $e Reader. (Normalized: Reader)  | 1   
Mapping failed for 700 $e Secretary [and compiler?]. (Normalized: Secretary and compiler)  | 1   
Mapping failed for 700 $e Series Consultant. (Normalized: Series Consultant)  | 1   
Mapping failed for 700 $e Series Editor. (Normalized: Series Editor)  | 1   
Mapping failed for 700 $e Series editor. (Normalized: Series editor)  | 3   
Mapping failed for 700 $e Star Trek. (Normalized: Star Trek)  | 1   
Mapping failed for 700 $e Trans. (Normalized: Trans)  | 2   
Mapping failed for 700 $e [ed.] (Normalized: ed)  | 1   
Mapping failed for 700 $e [ed.]. (Normalized: ed)  | 1   
Mapping failed for 700 $e [jt. ed.]. (Normalized: jt ed)  | 1   
Mapping failed for 700 $e aartist. (Normalized: aartist)  | 1   
Mapping failed for 700 $e abridger ; (Normalized: abridger )  | 1   
Mapping failed for 700 $e abridgment. (Normalized: abridgment)  | 2   
Mapping failed for 700 $e abriger. (Normalized: abriger)  | 1   
Mapping failed for 700 $e act (Normalized: act)  | 5   
Mapping failed for 700 $e act. (Normalized: act)  | 3   
Mapping failed for 700 $e acto. (Normalized: acto)  | 1   
Mapping failed for 700 $e actor.?UNAUTHORIZED (Normalized: actorUNAUTHORIZED)  | 2   
Mapping failed for 700 $e actress. (Normalized: actress)  | 2   
Mapping failed for 700 $e adap. (Normalized: adap)  | 1   
Mapping failed for 700 $e adapt. (Normalized: adapt)  | 10   
Mapping failed for 700 $e adaptor , (Normalized: adaptor )  | 2   
Mapping failed for 700 $e adaptor. (Normalized: adaptor)  | 14   
Mapping failed for 700 $e adp. (Normalized: adp)  | 41   
Mapping failed for 700 $e advisor (Normalized: advisor)  | 2   
Mapping failed for 700 $e advisor. (Normalized: advisor)  | 5   
Mapping failed for 700 $e advisors. (Normalized: advisors)  | 3   
Mapping failed for 700 $e aiilustrator. (Normalized: aiilustrator)  | 1   
Mapping failed for 700 $e animation director. (Normalized: animation director)  | 1   
Mapping failed for 700 $e apprec. (Normalized: apprec)  | 1   
Mapping failed for 700 $e aritist. (Normalized: aritist)  | 1   
Mapping failed for 700 $e arr. (Normalized: arr)  | 8   
Mapping failed for 700 $e arrang. (Normalized: arrang)  | 2   
Mapping failed for 700 $e arranger of music. (Normalized: arranger of music)  | 1   
Mapping failed for 700 $e artist, collection cover artist. (Normalized: artist collection cover artist)  | 1   
Mapping failed for 700 $e artwork. (Normalized: artwork)  | 3   
Mapping failed for 700 $e ass ed. (Normalized: ass ed)  | 1   
Mapping failed for 700 $e ass. ed. (Normalized: ass ed)  | 1   
Mapping failed for 700 $e ass.ed. (Normalized: assed)  | 2   
Mapping failed for 700 $e assistant director, (Normalized: assistant director)  | 1   
Mapping failed for 700 $e assistant editor (Normalized: assistant editor)  | 1   
Mapping failed for 700 $e assistant editor. (Normalized: assistant editor)  | 1   
Mapping failed for 700 $e assistant illustrator. (Normalized: assistant illustrator)  | 2   
Mapping failed for 700 $e assistant. (Normalized: assistant)  | 1   
Mapping failed for 700 $e associate ed. (Normalized: associate ed)  | 1   
Mapping failed for 700 $e associate editor. (Normalized: associate editor)  | 2   
Mapping failed for 700 $e associate producer. (Normalized: associate producer)  | 1   
Mapping failed for 700 $e associate project directors. (Normalized: associate project directors)  | 1   
Mapping failed for 700 $e asst. ed. (Normalized: asst ed)  | 6   
Mapping failed for 700 $e atlas adviser. (Normalized: atlas adviser)  | 1   
Mapping failed for 700 $e au. (Normalized: au)  | 72   
Mapping failed for 700 $e audio editor. (Normalized: audio editor)  | 2   
Mapping failed for 700 $e audio. (Normalized: audio)  | 5   
Mapping failed for 700 $e auhtor. (Normalized: auhtor)  | 1   
Mapping failed for 700 $e aurthor , (Normalized: aurthor )  | 1   
Mapping failed for 700 $e aut. (Normalized: aut)  | 55   
Mapping failed for 700 $e aut., ed. (Normalized: aut ed)  | 1   
Mapping failed for 700 $e aut.. (Normalized: aut)  | 1   
Mapping failed for 700 $e auteur. (Normalized: auteur)  | 1   
Mapping failed for 700 $e auth. (Normalized: auth)  | 2   
Mapping failed for 700 $e author , (Normalized: author )  | 3   
Mapping failed for 700 $e author ; (Normalized: author )  | 9   
Mapping failed for 700 $e author of afterword (Normalized: author of afterword)  | 1   
Mapping failed for 700 $e author of afterword. (Normalized: author of afterword)  | 2   
Mapping failed for 700 $e author of comic book. (Normalized: author of comic book)  | 2   
Mapping failed for 700 $e author of foreword (Normalized: author of foreword)  | 1   
Mapping failed for 700 $e author of foreword. (Normalized: author of foreword)  | 11   
Mapping failed for 700 $e author of introduction, etc. (Normalized: author of introduction etc)  | 11   
Mapping failed for 700 $e author of introduction. (Normalized: author of introduction)  | 10   
Mapping failed for 700 $e author of novel, (Normalized: author of novel)  | 1   
Mapping failed for 700 $e author of screenplay. (Normalized: author of screenplay)  | 5   
Mapping failed for 700 $e author photograph. (Normalized: author photograph)  | 1   
Mapping failed for 700 $e author(expression). (Normalized: authorexpression)  | 1   
Mapping failed for 700 $e author, photographer. (Normalized: author photographer)  | 1   
Mapping failed for 700 $e author. ?UNAUTHORIZED (Normalized: author UNAUTHORIZED)  | 1   
Mapping failed for 700 $e author.?UNAUTHORIZED (Normalized: authorUNAUTHORIZED)  | 3   
Mapping failed for 700 $e author.Z (Normalized: authorZ)  | 1   
Mapping failed for 700 $e authors. (Normalized: authors)  | 1   
Mapping failed for 700 $e autr. (Normalized: autr)  | 3   
Mapping failed for 700 $e bjd. (Normalized: bjd)  | 4   
Mapping failed for 700 $e bkd. (Normalized: bkd)  | 1   
Mapping failed for 700 $e book illustrator. (Normalized: book illustrator)  | 1   
Mapping failed for 700 $e breakdowns. (Normalized: breakdowns)  | 1   
Mapping failed for 700 $e bridgment. (Normalized: bridgment)  | 1   
Mapping failed for 700 $e camera (Normalized: camera)  | 1   
Mapping failed for 700 $e camera. (Normalized: camera)  | 1   
Mapping failed for 700 $e cameraman. (Normalized: cameraman)  | 1   
Mapping failed for 700 $e cartogropher. (Normalized: cartogropher)  | 3   
Mapping failed for 700 $e cartoonist. (Normalized: cartoonist)  | 2   
Mapping failed for 700 $e cartoons. (Normalized: cartoons)  | 1   
Mapping failed for 700 $e cast. (Normalized: cast)  | 3   
Mapping failed for 700 $e ccomposer, (Normalized: ccomposer)  | 2   
Mapping failed for 700 $e cellist. (Normalized: cellist)  | 1   
Mapping failed for 700 $e chairman (Normalized: chairman)  | 1   
Mapping failed for 700 $e chairman. (Normalized: chairman)  | 14   
Mapping failed for 700 $e chief contributing writer. (Normalized: chief contributing writer)  | 1   
Mapping failed for 700 $e chief editor. (Normalized: chief editor)  | 1   
Mapping failed for 700 $e chm. (Normalized: chm)  | 1   
Mapping failed for 700 $e cinematograper. (Normalized: cinematograper)  | 2   
Mapping failed for 700 $e cinematography. (Normalized: cinematography)  | 2   
Mapping failed for 700 $e cmm. (Normalized: cmm)  | 1   
Mapping failed for 700 $e co-ordinating producer. (Normalized: coordinating producer)  | 6   
Mapping failed for 700 $e co-ordinator. (Normalized: coordinator)  | 1   
Mapping failed for 700 $e co-producer. (Normalized: coproducer)  | 1   
Mapping failed for 700 $e co-writer, (Normalized: cowriter)  | 1   
Mapping failed for 700 $e coeditor. (Normalized: coeditor)  | 1   
Mapping failed for 700 $e col. (Normalized: col)  | 1   
Mapping failed for 700 $e col. ill. (Normalized: col ill)  | 19   
Mapping failed for 700 $e coll. (Normalized: coll)  | 1   
Mapping failed for 700 $e coll. ill. (Normalized: coll ill)  | 1   
Mapping failed for 700 $e collaborator. (Normalized: collaborator)  | 2   
Mapping failed for 700 $e collator (Normalized: collator)  | 1   
Mapping failed for 700 $e collection cover artist. (Normalized: collection cover artist)  | 3   
Mapping failed for 700 $e colorist.?UNAUTHORIZED (Normalized: coloristUNAUTHORIZED)  | 1   
Mapping failed for 700 $e colourer. (Normalized: colourer)  | 1   
Mapping failed for 700 $e colourist (Normalized: colourist)  | 30   
Mapping failed for 700 $e colourist, (Normalized: colourist)  | 19   
Mapping failed for 700 $e colourist, collection cover artist. (Normalized: colourist collection cover artist)  | 1   
Mapping failed for 700 $e colourist. (Normalized: colourist)  | 88   
Mapping failed for 700 $e colours (Normalized: colours)  | 1   
Mapping failed for 700 $e com (Normalized: com)  | 1   
Mapping failed for 700 $e com. (Normalized: com)  | 124   
Mapping failed for 700 $e comedian. (Normalized: comedian)  | 1   
Mapping failed for 700 $e commentato (Normalized: commentato)  | 1   
Mapping failed for 700 $e commenter, (Normalized: commenter)  | 2   
Mapping failed for 700 $e commenter. (Normalized: commenter)  | 20   
Mapping failed for 700 $e commissioner. (Normalized: commissioner)  | 2   
Mapping failed for 700 $e commmenter. (Normalized: commmenter)  | 17   
Mapping failed for 700 $e comp. & ed. (Normalized: comp  ed)  | 2   
Mapping failed for 700 $e comp. (Normalized: comp)  | 190   
Mapping failed for 700 $e comp. ed. (Normalized: comp ed)  | 2   
Mapping failed for 700 $e comp., (Normalized: comp)  | 1   
Mapping failed for 700 $e comp./ed. (Normalized: comped)  | 1   
Mapping failed for 700 $e compil. (Normalized: compil)  | 1   
Mapping failed for 700 $e compiler and editor. (Normalized: compiler and editor)  | 1   
Mapping failed for 700 $e compiler of bibliography. (Normalized: compiler of bibliography)  | 1   
Mapping failed for 700 $e complier. (Normalized: complier)  | 2   
Mapping failed for 700 $e composer (expression) (Normalized: composer expression)  | 169   
Mapping failed for 700 $e composer (expression), (Normalized: composer expression)  | 6   
Mapping failed for 700 $e composer (expression). (Normalized: composer expression)  | 10   
Mapping failed for 700 $e composer (expression.) (Normalized: composer expression)  | 2   
Mapping failed for 700 $e comps. (Normalized: comps)  | 1   
Mapping failed for 700 $e conpiler. (Normalized: conpiler)  | 1   
Mapping failed for 700 $e cons ed. (Normalized: cons ed)  | 2   
Mapping failed for 700 $e cons. ed. (Normalized: cons ed)  | 1   
Mapping failed for 700 $e constr. (Normalized: constr)  | 1   
Mapping failed for 700 $e consul. (Normalized: consul)  | 1   
Mapping failed for 700 $e consult. (Normalized: consult)  | 2   
Mapping failed for 700 $e consultant ed. (Normalized: consultant ed)  | 1   
Mapping failed for 700 $e cont. (Normalized: cont)  | 10   
Mapping failed for 700 $e contrib. (Normalized: contrib)  | 4   
Mapping failed for 700 $e contrib. au. (Normalized: contrib au)  | 1   
Mapping failed for 700 $e contrib. ed. (Normalized: contrib ed)  | 3   
Mapping failed for 700 $e contrib., ed. (Normalized: contrib ed)  | 1   
Mapping failed for 700 $e contributer. (Normalized: contributer)  | 4   
Mapping failed for 700 $e contributing ed. (Normalized: contributing ed)  | 1   
Mapping failed for 700 $e contributing editor. (Normalized: contributing editor)  | 1   
Mapping failed for 700 $e contributing researchers. (Normalized: contributing researchers)  | 1   
Mapping failed for 700 $e contributor.?UNAUTHORIZED (Normalized: contributorUNAUTHORIZED)  | 1   
Mapping failed for 700 $e contritutor. (Normalized: contritutor)  | 1   
Mapping failed for 700 $e coordinator. (Normalized: coordinator)  | 1   
Mapping failed for 700 $e copy editor. (Normalized: copy editor)  | 3   
Mapping failed for 700 $e costume desinger. (Normalized: costume desinger)  | 1   
Mapping failed for 700 $e cover artist. (Normalized: cover artist)  | 7   
Mapping failed for 700 $e cover colourist. (Normalized: cover colourist)  | 1   
Mapping failed for 700 $e cover ill. (Normalized: cover ill)  | 1   
Mapping failed for 700 $e cover illustrator. (Normalized: cover illustrator)  | 9   
Mapping failed for 700 $e creat. (Normalized: creat)  | 1   
Mapping failed for 700 $e creative director. (Normalized: creative director)  | 2   
Mapping failed for 700 $e creator ; (Normalized: creator )  | 1   
Mapping failed for 700 $e creator of television series. (Normalized: creator of television series)  | 1   
Mapping failed for 700 $e creator, designer. (Normalized: creator designer)  | 1   
Mapping failed for 700 $e csl. (Normalized: csl)  | 3   
Mapping failed for 700 $e custume designer. (Normalized: custume designer)  | 1   
Mapping failed for 700 $e d. (Normalized: d)  | 17   
Mapping failed for 700 $e d.. (Normalized: d)  | 1   
Mapping failed for 700 $e ded. (Normalized: ded)  | 1   
Mapping failed for 700 $e des. (Normalized: des)  | 1   
Mapping failed for 700 $e desig. (Normalized: desig)  | 1   
Mapping failed for 700 $e design. (Normalized: design)  | 1   
Mapping failed for 700 $e designed by. (Normalized: designed by)  | 1   
Mapping failed for 700 $e designer ; (Normalized: designer )  | 1   
Mapping failed for 700 $e designer, ill. (Normalized: designer ill)  | 2   
Mapping failed for 700 $e designing. (Normalized: designing)  | 3   
Mapping failed for 700 $e dib. (Normalized: dib)  | 1   
Mapping failed for 700 $e diector. (Normalized: diector)  | 1   
Mapping failed for 700 $e dir. (Normalized: dir)  | 8   
Mapping failed for 700 $e directed, (Normalized: directed)  | 1   
Mapping failed for 700 $e directed. (Normalized: directed)  | 6   
Mapping failed for 700 $e direction. (Normalized: direction)  | 2   
Mapping failed for 700 $e director , (Normalized: director )  | 7   
Mapping failed for 700 $e director ; (Normalized: director )  | 17   
Mapping failed for 700 $e director and producer. (Normalized: director and producer)  | 2   
Mapping failed for 700 $e director of photographer. (Normalized: director of photographer)  | 1   
Mapping failed for 700 $e director of photography (Normalized: director of photography)  | 10   
Mapping failed for 700 $e director of photography, (Normalized: director of photography)  | 3   
Mapping failed for 700 $e director of photography. (Normalized: director of photography)  | 155   
Mapping failed for 700 $e director or photography (Normalized: director or photography)  | 1   
Mapping failed for 700 $e director or photography. (Normalized: director or photography)  | 1   
Mapping failed for 700 $e director. ; (Normalized: director )  | 1   
Mapping failed for 700 $e director.?UNAUTHORIZED (Normalized: directorUNAUTHORIZED)  | 1   
Mapping failed for 700 $e diredctor. (Normalized: diredctor)  | 1   
Mapping failed for 700 $e ditor of compilation. (Normalized: ditor of compilation)  | 2   
Mapping failed for 700 $e ditor, (Normalized: ditor)  | 2   
Mapping failed for 700 $e ditor. (Normalized: ditor)  | 40   
Mapping failed for 700 $e dsr. (Normalized: dsr)  | 6   
Mapping failed for 700 $e e illustrator. (Normalized: e illustrator)  | 1   
Mapping failed for 700 $e eauthor, (Normalized: eauthor)  | 1   
Mapping failed for 700 $e ed (Normalized: ed)  | 11   
Mapping failed for 700 $e ed dir. (Normalized: ed dir)  | 1   
Mapping failed for 700 $e ed. (Normalized: ed)  | 3,903   
Mapping failed for 700 $e ed. , intro. (Normalized: ed  intro)  | 1   
Mapping failed for 700 $e ed. and tr. (Normalized: ed and tr)  | 5   
Mapping failed for 700 $e ed. and trans. (Normalized: ed and trans)  | 1   
Mapping failed for 700 $e ed. in chief. (Normalized: ed in chief)  | 2   
Mapping failed for 700 $e ed., (Normalized: ed)  | 3   
Mapping failed for 700 $e ed., abridged. (Normalized: ed abridged)  | 1   
Mapping failed for 700 $e ed., commentary. (Normalized: ed commentary)  | 2   
Mapping failed for 700 $e ed., computer notation. (Normalized: ed computer notation)  | 1   
Mapping failed for 700 $e ed., con. (Normalized: ed con)  | 1   
Mapping failed for 700 $e ed., into. (Normalized: ed into)  | 1   
Mapping failed for 700 $e ed., intro. (Normalized: ed intro)  | 3   
Mapping failed for 700 $e ed., pub. (Normalized: ed pub)  | 1   
Mapping failed for 700 $e ed., res. (Normalized: ed res)  | 1   
Mapping failed for 700 $e ed., trans. (Normalized: ed trans)  | 2   
Mapping failed for 700 $e ed.- (Normalized: ed)  | 1   
Mapping failed for 700 $e ed.. (Normalized: ed)  | 9   
Mapping failed for 700 $e ed.?UNAUTHORIZED (Normalized: edUNAUTHORIZED)  | 3   
Mapping failed for 700 $e edirector, (Normalized: edirector)  | 1   
Mapping failed for 700 $e edirector. (Normalized: edirector)  | 1   
Mapping failed for 700 $e edit. (Normalized: edit)  | 1   
Mapping failed for 700 $e edited. (Normalized: edited)  | 1   
Mapping failed for 700 $e editing ; (Normalized: editing )  | 3   
Mapping failed for 700 $e editing. (Normalized: editing)  | 2   
Mapping failed for 700 $e editor & prnicipal contributor. (Normalized: editor  prnicipal contributor)  | 1   
Mapping failed for 700 $e editor ; (Normalized: editor )  | 2   
Mapping failed for 700 $e editor-coordinator. (Normalized: editorcoordinator)  | 1   
Mapping failed for 700 $e editor.?UNAUTHORIZED (Normalized: editorUNAUTHORIZED)  | 1   
Mapping failed for 700 $e editorial consultant (revised edition) (Normalized: editorial consultant revised edition)  | 1   
Mapping failed for 700 $e editorial coordination. (Normalized: editorial coordination)  | 1   
Mapping failed for 700 $e editors. (Normalized: editors)  | 2   
Mapping failed for 700 $e edt. (Normalized: edt)  | 6   
Mapping failed for 700 $e ee. (Normalized: ee)  | 1   
Mapping failed for 700 $e eed. (Normalized: eed)  | 5   
Mapping failed for 700 $e eeditor. (Normalized: eeditor)  | 1   
Mapping failed for 700 $e eexecutive producer. (Normalized: eexecutive producer)  | 1   
Mapping failed for 700 $e eiditor. (Normalized: eiditor)  | 1   
Mapping failed for 700 $e eill. (Normalized: eill)  | 1   
Mapping failed for 700 $e enarrator. (Normalized: enarrator)  | 2   
Mapping failed for 700 $e eproducer. (Normalized: eproducer)  | 1   
Mapping failed for 700 $e exceutive producer. (Normalized: exceutive producer)  | 2   
Mapping failed for 700 $e excutive producer. (Normalized: excutive producer)  | 3   
Mapping failed for 700 $e execitive producer. (Normalized: execitive producer)  | 2   
Mapping failed for 700 $e execuitive producer. (Normalized: execuitive producer)  | 1   
Mapping failed for 700 $e executed producer. (Normalized: executed producer)  | 1   
Mapping failed for 700 $e executice producer. (Normalized: executice producer)  | 1   
Mapping failed for 700 $e executive  editor. (Normalized: executive  editor)  | 1   
Mapping failed for 700 $e executive (Normalized: executive)  | 1   
Mapping failed for 700 $e executive directive. (Normalized: executive directive)  | 1   
Mapping failed for 700 $e executive director. (Normalized: executive director)  | 3   
Mapping failed for 700 $e executive procuder. (Normalized: executive procuder)  | 1   
Mapping failed for 700 $e executive prodcucer. (Normalized: executive prodcucer)  | 1   
Mapping failed for 700 $e executive prodcuer. (Normalized: executive prodcuer)  | 2   
Mapping failed for 700 $e executive produced. (Normalized: executive produced)  | 2   
Mapping failed for 700 $e executive producer (Normalized: executive producer)  | 16   
Mapping failed for 700 $e executive producer , (Normalized: executive producer )  | 4   
Mapping failed for 700 $e executive producer ; (Normalized: executive producer )  | 17   
Mapping failed for 700 $e executive producer and director (Normalized: executive producer and director)  | 1   
Mapping failed for 700 $e executive producer and director. (Normalized: executive producer and director)  | 2   
Mapping failed for 700 $e executive producer and producer. (Normalized: executive producer and producer)  | 1   
Mapping failed for 700 $e executive producer, (Normalized: executive producer)  | 3   
Mapping failed for 700 $e executive producer, director. (Normalized: executive producer director)  | 1   
Mapping failed for 700 $e executive producer. (Normalized: executive producer)  | 916   
Mapping failed for 700 $e executive producers (Normalized: executive producers)  | 3   
Mapping failed for 700 $e executive producers. (Normalized: executive producers)  | 11   
Mapping failed for 700 $e executive production. (Normalized: executive production)  | 1   
Mapping failed for 700 $e executive productive. (Normalized: executive productive)  | 1   
Mapping failed for 700 $e executive. (Normalized: executive)  | 8   
Mapping failed for 700 $e expanded version of. (Normalized: expanded version of)  | 1   
Mapping failed for 700 $e éd. (Normalized: ed)  | 2   
Mapping failed for 700 $e film composer. (Normalized: film composer)  | 1   
Mapping failed for 700 $e film direcor. (Normalized: film direcor)  | 1   
Mapping failed for 700 $e film director ; (Normalized: film director )  | 1   
Mapping failed for 700 $e film maker,  (Normalized: film maker)  | 1   
Mapping failed for 700 $e film proudcer, (Normalized: film proudcer)  | 1   
Mapping failed for 700 $e film. (Normalized: film)  | 1   
Mapping failed for 700 $e filmeditor. (Normalized: filmeditor)  | 4   
Mapping failed for 700 $e flm (Normalized: flm)  | 1   
Mapping failed for 700 $e foreword. (Normalized: foreword)  | 4   
Mapping failed for 700 $e forwd. (Normalized: forwd)  | 1   
Mapping failed for 700 $e founder of work. (Normalized: founder of work)  | 2   
Mapping failed for 700 $e fwd. (Normalized: fwd)  | 39   
Mapping failed for 700 $e gen ed. (Normalized: gen ed)  | 2   
Mapping failed for 700 $e gen. ed. (Normalized: gen ed)  | 1   
Mapping failed for 700 $e gen. editor. (Normalized: gen editor)  | 2   
Mapping failed for 700 $e general ed. (Normalized: general ed)  | 5   
Mapping failed for 700 $e general editor. (Normalized: general editor)  | 4   
Mapping failed for 700 $e graphic artist. (Normalized: graphic artist)  | 1   
Mapping failed for 700 $e graphic design. (Normalized: graphic design)  | 1   
Mapping failed for 700 $e graphics and photography. (Normalized: graphics and photography)  | 1   
Mapping failed for 700 $e graphics designer. (Normalized: graphics designer)  | 1   
Mapping failed for 700 $e graphics. (Normalized: graphics)  | 1   
Mapping failed for 700 $e guitarist. (Normalized: guitarist)  | 2   
Mapping failed for 700 $e i ll. (Normalized: i ll)  | 2   
Mapping failed for 700 $e iil (Normalized: iil)  | 1   
Mapping failed for 700 $e iil. (Normalized: iil)  | 1   
Mapping failed for 700 $e iill. (Normalized: iill)  | 1   
Mapping failed for 700 $e iilustrator. (Normalized: iilustrator)  | 1   
Mapping failed for 700 $e il. (Normalized: il)  | 6   
Mapping failed for 700 $e ill (Normalized: ill)  | 209   
Mapping failed for 700 $e ill, (Normalized: ill)  | 2   
Mapping failed for 700 $e ill. (Normalized: ill)  | 12,198   
Mapping failed for 700 $e ill. , photo. (Normalized: ill  photo)  | 1   
Mapping failed for 700 $e ill. . (Normalized: ill )  | 9   
Mapping failed for 700 $e ill. NAR needed (Normalized: ill NAR needed)  | 1   
Mapping failed for 700 $e ill. adapt. (Normalized: ill adapt)  | 1   
Mapping failed for 700 $e ill., (Normalized: ill)  | 3   
Mapping failed for 700 $e ill., jt au. (Normalized: ill jt au)  | 1   
Mapping failed for 700 $e ill., photo. (Normalized: ill photo)  | 2   
Mapping failed for 700 $e ill., script. (Normalized: ill script)  | 1   
Mapping failed for 700 $e ill., story. (Normalized: ill story)  | 2   
Mapping failed for 700 $e ill.. (Normalized: ill)  | 8   
Mapping failed for 700 $e ill.?UNAUTHORIZED (Normalized: illUNAUTHORIZED)  | 1   
Mapping failed for 700 $e illistrator. (Normalized: illistrator)  | 8   
Mapping failed for 700 $e illlustrator. (Normalized: illlustrator)  | 4   
Mapping failed for 700 $e ills. (Normalized: ills)  | 1   
Mapping failed for 700 $e illuatrator. (Normalized: illuatrator)  | 1   
Mapping failed for 700 $e illurstator (Normalized: illurstator)  | 1   
Mapping failed for 700 $e illus. (Normalized: illus)  | 131   
Mapping failed for 700 $e illus.. (Normalized: illus)  | 1   
Mapping failed for 700 $e illusrtator. (Normalized: illusrtator)  | 1   
Mapping failed for 700 $e illustator. (Normalized: illustator)  | 6   
Mapping failed for 700 $e illustrated. (Normalized: illustrated)  | 1   
Mapping failed for 700 $e illustration. (Normalized: illustration)  | 1   
Mapping failed for 700 $e illustrations (Normalized: illustrations)  | 4   
Mapping failed for 700 $e illustrations. (Normalized: illustrations)  | 9   
Mapping failed for 700 $e illustratior (Normalized: illustratior)  | 1   
Mapping failed for 700 $e illustratior. (Normalized: illustratior)  | 2   
Mapping failed for 700 $e illustratoer. (Normalized: illustratoer)  | 1   
Mapping failed for 700 $e illustrator ?UNAUTHORIZED (Normalized: illustrator UNAUTHORIZED)  | 1   
Mapping failed for 700 $e illustrator.?UNAUTHORIZED (Normalized: illustratorUNAUTHORIZED)  | 3   
Mapping failed for 700 $e illustrator.MN (Normalized: illustratorMN)  | 1   
Mapping failed for 700 $e illustrator?UNAUTHORIZED (Normalized: illustratorUNAUTHORIZED)  | 2   
Mapping failed for 700 $e illustrtions. (Normalized: illustrtions)  | 1   
Mapping failed for 700 $e illutrator. (Normalized: illutrator)  | 2   
Mapping failed for 700 $e ilustrator. (Normalized: ilustrator)  | 1   
Mapping failed for 700 $e ink art. (Normalized: ink art)  | 1   
Mapping failed for 700 $e inker (Normalized: inker)  | 17   
Mapping failed for 700 $e inker, (Normalized: inker)  | 4   
Mapping failed for 700 $e inker, collection cover artist. (Normalized: inker collection cover artist)  | 1   
Mapping failed for 700 $e inker. (Normalized: inker)  | 33   
Mapping failed for 700 $e inker/finisher. (Normalized: inkerfinisher)  | 2   
Mapping failed for 700 $e inkers (Normalized: inkers)  | 1   
Mapping failed for 700 $e inspiration of work. (Normalized: inspiration of work)  | 1   
Mapping failed for 700 $e int. (Normalized: int)  | 1   
Mapping failed for 700 $e interior illustrator (Normalized: interior illustrator)  | 1   
Mapping failed for 700 $e interior illustrator?UNAUTHORIZED (Normalized: interior illustratorUNAUTHORIZED)  | 1   
Mapping failed for 700 $e interpreter (Normalized: interpreter)  | 1   
Mapping failed for 700 $e interpreter. (Normalized: interpreter)  | 20   
Mapping failed for 700 $e interveiwee (Normalized: interveiwee)  | 1   
Mapping failed for 700 $e interveiwee. (Normalized: interveiwee)  | 18   
Mapping failed for 700 $e interveiwer. (Normalized: interveiwer)  | 4   
Mapping failed for 700 $e interview. (Normalized: interview)  | 2   
Mapping failed for 700 $e interviewee (expression) (Normalized: interviewee expression)  | 18   
Mapping failed for 700 $e intro. (Normalized: intro)  | 20   
Mapping failed for 700 $e intro. , notes. (Normalized: intro  notes)  | 1   
Mapping failed for 700 $e intro., ed. (Normalized: intro ed)  | 1   
Mapping failed for 700 $e introd. (Normalized: introd)  | 1   
Mapping failed for 700 $e ive (Normalized: ive)  | 1   
Mapping failed for 700 $e j aut. (Normalized: j aut)  | 1   
Mapping failed for 700 $e jacket design (Normalized: jacket design)  | 1   
Mapping failed for 700 $e jacket designer. (Normalized: jacket designer)  | 1   
Mapping failed for 700 $e joint  author. (Normalized: joint  author)  | 1   
Mapping failed for 700 $e joint author (Normalized: joint author)  | 2   
Mapping failed for 700 $e joint author. (Normalized: joint author)  | 492   
Mapping failed for 700 $e joint comp. (Normalized: joint comp)  | 20   
Mapping failed for 700 $e joint ed. (Normalized: joint ed)  | 25   
Mapping failed for 700 $e joint editor. (Normalized: joint editor)  | 3   
Mapping failed for 700 $e joint tr. (Normalized: joint tr)  | 5   
Mapping failed for 700 $e joint. author. (Normalized: joint author)  | 1   
Mapping failed for 700 $e journalist, (Normalized: journalist)  | 1   
Mapping failed for 700 $e journalist. (Normalized: journalist)  | 3   
Mapping failed for 700 $e jt au. (Normalized: jt au)  | 421   
Mapping failed for 700 $e jt au., ed. (Normalized: jt au ed)  | 1   
Mapping failed for 700 $e jt aut. (Normalized: jt aut)  | 53   
Mapping failed for 700 $e jt aut.. (Normalized: jt aut)  | 1   
Mapping failed for 700 $e jt auth. (Normalized: jt auth)  | 3   
Mapping failed for 700 $e jt author. (Normalized: jt author)  | 2   
Mapping failed for 700 $e jt autr. (Normalized: jt autr)  | 7   
Mapping failed for 700 $e jt biogr. (Normalized: jt biogr)  | 1   
Mapping failed for 700 $e jt comp. (Normalized: jt comp)  | 1   
Mapping failed for 700 $e jt ed.. (Normalized: jt ed)  | 2   
Mapping failed for 700 $e jt su. (Normalized: jt su)  | 1   
Mapping failed for 700 $e jt trans. (Normalized: jt trans)  | 2   
Mapping failed for 700 $e jt, aut. (Normalized: jt aut)  | 1   
Mapping failed for 700 $e jt,aut. (Normalized: jtaut)  | 1   
Mapping failed for 700 $e jt,auth. (Normalized: jtauth)  | 1   
Mapping failed for 700 $e jt. Cut. (Normalized: jt Cut)  | 1   
Mapping failed for 700 $e jt. adaptor. (Normalized: jt adaptor)  | 1   
Mapping failed for 700 $e jt. at. (Normalized: jt at)  | 1   
Mapping failed for 700 $e jt. au. (Normalized: jt au)  | 309   
Mapping failed for 700 $e jt. au. and ed. (Normalized: jt au and ed)  | 1   
Mapping failed for 700 $e jt. aut . (Normalized: jt aut )  | 1   
Mapping failed for 700 $e jt. aut. & ill. (Normalized: jt aut  ill)  | 1   
Mapping failed for 700 $e jt. aut. (Normalized: jt aut)  | 2,238   
Mapping failed for 700 $e jt. aut. . (Normalized: jt aut )  | 2   
Mapping failed for 700 $e jt. aut., (Normalized: jt aut)  | 2   
Mapping failed for 700 $e jt. aut., ill. (Normalized: jt aut ill)  | 1   
Mapping failed for 700 $e jt. aut.. (Normalized: jt aut)  | 5   
Mapping failed for 700 $e jt. auth. (Normalized: jt auth)  | 94   
Mapping failed for 700 $e jt. author. (Normalized: jt author)  | 171   
Mapping failed for 700 $e jt. authors. (Normalized: jt authors)  | 1   
Mapping failed for 700 $e jt. autr. (Normalized: jt autr)  | 65   
Mapping failed for 700 $e jt. biograp. (Normalized: jt biograp)  | 1   
Mapping failed for 700 $e jt. com. (Normalized: jt com)  | 2   
Mapping failed for 700 $e jt. comp. (Normalized: jt comp)  | 13   
Mapping failed for 700 $e jt. creator of Chic Simple Series of guides to modern-day living. (Normalized: jt creator of Chic Simple Series of guides to modernday living)  | 2   
Mapping failed for 700 $e jt. ed. (Normalized: jt ed)  | 136   
Mapping failed for 700 $e jt. editor. (Normalized: jt editor)  | 10   
Mapping failed for 700 $e jt. ill. (Normalized: jt ill)  | 3   
Mapping failed for 700 $e jt. producer. (Normalized: jt producer)  | 1   
Mapping failed for 700 $e jt. series editor. (Normalized: jt series editor)  | 1   
Mapping failed for 700 $e jt. trans. (Normalized: jt trans)  | 3   
Mapping failed for 700 $e jt.au. (Normalized: jtau)  | 91   
Mapping failed for 700 $e jt.aut, (Normalized: jtaut)  | 1   
Mapping failed for 700 $e jt.aut. (Normalized: jtaut)  | 615   
Mapping failed for 700 $e jt.aut.. (Normalized: jtaut)  | 1   
Mapping failed for 700 $e jt.auth. (Normalized: jtauth)  | 5   
Mapping failed for 700 $e jt.author. (Normalized: jtauthor)  | 8   
Mapping failed for 700 $e jt.ayt. (Normalized: jtayt)  | 1   
Mapping failed for 700 $e jt.ed. (Normalized: jted)  | 7   
Mapping failed for 700 $e jtau. (Normalized: jtau)  | 1   
Mapping failed for 700 $e lang. cons. (Normalized: lang cons)  | 1   
Mapping failed for 700 $e layouter. (Normalized: layouter)  | 2   
Mapping failed for 700 $e lecture. (Normalized: lecture)  | 1   
Mapping failed for 700 $e lecturer. (Normalized: lecturer)  | 1   
Mapping failed for 700 $e letter (Normalized: letter)  | 8   
Mapping failed for 700 $e letter. (Normalized: letter)  | 10   
Mapping failed for 700 $e letterer (Normalized: letterer)  | 7   
Mapping failed for 700 $e letterer. (Normalized: letterer)  | 165   
Mapping failed for 700 $e lettering. (Normalized: lettering)  | 1   
Mapping failed for 700 $e letters. (Normalized: letters)  | 2   
Mapping failed for 700 $e live concert producer. (Normalized: live concert producer)  | 1   
Mapping failed for 700 $e lyracist. (Normalized: lyracist)  | 1   
Mapping failed for 700 $e m (Normalized: m)  | 1   
Mapping failed for 700 $e map and chapter opener ill. (Normalized: map and chapter opener ill)  | 1   
Mapping failed for 700 $e map ill. (Normalized: map ill)  | 1   
Mapping failed for 700 $e martial artist. (Normalized: martial artist)  | 4   
Mapping failed for 700 $e master. (Normalized: master)  | 1   
Mapping failed for 700 $e mixer ; (Normalized: mixer )  | 1   
Mapping failed for 700 $e music arranger. (Normalized: music arranger)  | 2   
Mapping failed for 700 $e music composer. (Normalized: music composer)  | 4   
Mapping failed for 700 $e music performer. (Normalized: music performer)  | 1   
Mapping failed for 700 $e music producer. (Normalized: music producer)  | 1   
Mapping failed for 700 $e music. (Normalized: music)  | 16   
Mapping failed for 700 $e musical arranger. (Normalized: musical arranger)  | 1   
Mapping failed for 700 $e musical composer , (Normalized: musical composer )  | 1   
Mapping failed for 700 $e musical composer. (Normalized: musical composer)  | 1   
Mapping failed for 700 $e musical director , (Normalized: musical director )  | 1   
Mapping failed for 700 $e musician (expression) (Normalized: musician expression)  | 1   
Mapping failed for 700 $e musician (expression). (Normalized: musician expression)  | 1   
Mapping failed for 700 $e musician ; (Normalized: musician )  | 2   
Mapping failed for 700 $e musicians. (Normalized: musicians)  | 2   
Mapping failed for 700 $e música. (Normalized: musica)  | 2   
Mapping failed for 700 $e narator. (Normalized: narator)  | 1   
Mapping failed for 700 $e narration. (Normalized: narration)  | 1   
Mapping failed for 700 $e narrator ; (Normalized: narrator )  | 3   
Mapping failed for 700 $e narrator.?UNAUTHORIZED (Normalized: narratorUNAUTHORIZED)  | 2   
Mapping failed for 700 $e narrrator (Normalized: narrrator)  | 1   
Mapping failed for 700 $e notes. (Normalized: notes)  | 1   
Mapping failed for 700 $e nrt. (Normalized: nrt)  | 31   
Mapping failed for 700 $e on-screen participant, (Normalized: onscreen participant)  | 1   
Mapping failed for 700 $e on-screen participant. (Normalized: onscreen participant)  | 5   
Mapping failed for 700 $e organisation. (Normalized: organisation)  | 1   
Mapping failed for 700 $e paintings. (Normalized: paintings)  | 1   
Mapping failed for 700 $e participant. (Normalized: participant)  | 2   
Mapping failed for 700 $e penciler. (Normalized: penciler)  | 6   
Mapping failed for 700 $e penciller (Normalized: penciller)  | 9   
Mapping failed for 700 $e penciller, (Normalized: penciller)  | 10   
Mapping failed for 700 $e penciller. (Normalized: penciller)  | 27   
Mapping failed for 700 $e penguin producer (Normalized: penguin producer)  | 1   
Mapping failed for 700 $e penguin producer. (Normalized: penguin producer)  | 1   
Mapping failed for 700 $e percussion. (Normalized: percussion)  | 2   
Mapping failed for 700 $e perfomer. (Normalized: perfomer)  | 1   
Mapping failed for 700 $e phot. (Normalized: phot)  | 1   
Mapping failed for 700 $e photo. (Normalized: photo)  | 45   
Mapping failed for 700 $e photo. ed. (Normalized: photo ed)  | 1   
Mapping failed for 700 $e photog. (Normalized: photog)  | 24   
Mapping failed for 700 $e photograher. (Normalized: photograher)  | 1   
Mapping failed for 700 $e photograper. (Normalized: photograper)  | 1   
Mapping failed for 700 $e photographer (expression) (Normalized: photographer expression)  | 3   
Mapping failed for 700 $e photographer director (Normalized: photographer director)  | 1   
Mapping failed for 700 $e photographs. (Normalized: photographs)  | 2   
Mapping failed for 700 $e photography. (Normalized: photography)  | 3   
Mapping failed for 700 $e photos. (Normalized: photos)  | 24   
Mapping failed for 700 $e pht. (Normalized: pht)  | 109   
Mapping failed for 700 $e poet. (Normalized: poet)  | 1   
Mapping failed for 700 $e post-production. (Normalized: postproduction)  | 1   
Mapping failed for 700 $e pref. (Normalized: pref)  | 1   
Mapping failed for 700 $e preface. (Normalized: preface)  | 1   
Mapping failed for 700 $e prf (Normalized: prf)  | 7   
Mapping failed for 700 $e prf. (Normalized: prf)  | 17   
Mapping failed for 700 $e pro. (Normalized: pro)  | 1   
Mapping failed for 700 $e procuder. (Normalized: procuder)  | 1   
Mapping failed for 700 $e prod. (Normalized: prod)  | 4   
Mapping failed for 700 $e prodcuer ; (Normalized: prodcuer )  | 1   
Mapping failed for 700 $e prodcuer and director (Normalized: prodcuer and director)  | 1   
Mapping failed for 700 $e prodcuer. (Normalized: prodcuer)  | 2   
Mapping failed for 700 $e produce. (Normalized: produce)  | 1   
Mapping failed for 700 $e produced ; (Normalized: produced )  | 1   
Mapping failed for 700 $e produced. (Normalized: produced)  | 1   
Mapping failed for 700 $e producer , (Normalized: producer )  | 33   
Mapping failed for 700 $e producer ; (Normalized: producer )  | 105   
Mapping failed for 700 $e producer and camera. (Normalized: producer and camera)  | 1   
Mapping failed for 700 $e producer and director (Normalized: producer and director)  | 11   
Mapping failed for 700 $e producer and director. (Normalized: producer and director)  | 13   
Mapping failed for 700 $e producer and ditrector (Normalized: producer and ditrector)  | 1   
Mapping failed for 700 $e producer, arranger. (Normalized: producer arranger)  | 1   
Mapping failed for 700 $e producer, co-ordinator, director. (Normalized: producer coordinator director)  | 1   
Mapping failed for 700 $e producer, director. (Normalized: producer director)  | 1   
Mapping failed for 700 $e producer, edirector. (Normalized: producer edirector)  | 1   
Mapping failed for 700 $e producer, film director, screenwriter, editor, actor. (Normalized: producer film director screenwriter editor actor)  | 1   
Mapping failed for 700 $e producer, songwriter. (Normalized: producer songwriter)  | 1   
Mapping failed for 700 $e producer.?UNAUTHORIZED (Normalized: producerUNAUTHORIZED)  | 1   
Mapping failed for 700 $e production (Normalized: production)  | 1   
Mapping failed for 700 $e production assistant. (Normalized: production assistant)  | 1   
Mapping failed for 700 $e production assistants. (Normalized: production assistants)  | 3   
Mapping failed for 700 $e production coordinator. (Normalized: production coordinator)  | 3   
Mapping failed for 700 $e production designe (Normalized: production designe)  | 1   
Mapping failed for 700 $e production supervisor (Normalized: production supervisor)  | 2   
Mapping failed for 700 $e production supervisor. (Normalized: production supervisor)  | 6   
Mapping failed for 700 $e production-co-ordinator. (Normalized: productioncoordinator)  | 1   
Mapping failed for 700 $e production. (Normalized: production)  | 13   
Mapping failed for 700 $e prog. aut. (Normalized: prog aut)  | 1   
Mapping failed for 700 $e project ed. (Normalized: project ed)  | 6   
Mapping failed for 700 $e pról. (Normalized: prol)  | 1   
Mapping failed for 700 $e pseud. (Normalized: pseud)  | 4   
Mapping failed for 700 $e pseudonym. (Normalized: pseudonym)  | 4   
Mapping failed for 700 $e pub. (Normalized: pub)  | 1   
Mapping failed for 700 $e reader (Normalized: reader)  | 1   
Mapping failed for 700 $e reader. (Normalized: reader)  | 1   
Mapping failed for 700 $e reading  consultant. (Normalized: reading  consultant)  | 1   
Mapping failed for 700 $e res. (Normalized: res)  | 5   
Mapping failed for 700 $e rev. (Normalized: rev)  | 4   
Mapping failed for 700 $e rev. au. (Normalized: rev au)  | 1   
Mapping failed for 700 $e revised ed. (Normalized: revised ed)  | 1   
Mapping failed for 700 $e revisor. (Normalized: revisor)  | 1   
Mapping failed for 700 $e revs. (Normalized: revs)  | 1   
Mapping failed for 700 $e sceenwriter. (Normalized: sceenwriter)  | 2   
Mapping failed for 700 $e scorer. (Normalized: scorer)  | 1   
Mapping failed for 700 $e screeenplay. (Normalized: screeenplay)  | 1   
Mapping failed for 700 $e screenplay (Normalized: screenplay)  | 1   
Mapping failed for 700 $e screenplay author. (Normalized: screenplay author)  | 3   
Mapping failed for 700 $e screenplay. (Normalized: screenplay)  | 4   
Mapping failed for 700 $e screenwiter, (Normalized: screenwiter)  | 1   
Mapping failed for 700 $e screenwritier, (Normalized: screenwritier)  | 1   
Mapping failed for 700 $e script (Normalized: script)  | 1   
Mapping failed for 700 $e script writer. (Normalized: script writer)  | 1   
Mapping failed for 700 $e scriptwriter. (Normalized: scriptwriter)  | 1   
Mapping failed for 700 $e sel., ed. (Normalized: sel ed)  | 2   
Mapping failed for 700 $e selector, (Normalized: selector)  | 1   
Mapping failed for 700 $e selector. (Normalized: selector)  | 4   
Mapping failed for 700 $e senior cookery ed. (Normalized: senior cookery ed)  | 1   
Mapping failed for 700 $e senior fellow. (Normalized: senior fellow)  | 1   
Mapping failed for 700 $e senior producer. (Normalized: senior producer)  | 1   
Mapping failed for 700 $e sequence director. (Normalized: sequence director)  | 2   
Mapping failed for 700 $e ser ed. (Normalized: ser ed)  | 1   
Mapping failed for 700 $e series author. (Normalized: series author)  | 3   
Mapping failed for 700 $e series consultant. (Normalized: series consultant)  | 3   
Mapping failed for 700 $e series ed. (Normalized: series ed)  | 47   
Mapping failed for 700 $e series editor. (Normalized: series editor)  | 20   
Mapping failed for 700 $e series producer and producer. (Normalized: series producer and producer)  | 1   
Mapping failed for 700 $e series producer. (Normalized: series producer)  | 12   
Mapping failed for 700 $e series. (Normalized: series)  | 1   
Mapping failed for 700 $e songwriter, arranger. (Normalized: songwriter arranger)  | 1   
Mapping failed for 700 $e soprano pan. (Normalized: soprano pan)  | 1   
Mapping failed for 700 $e special effects. (Normalized: special effects)  | 1   
Mapping failed for 700 $e still photography. (Normalized: still photography)  | 1   
Mapping failed for 700 $e storyline. (Normalized: storyline)  | 2   
Mapping failed for 700 $e sub-editor. (Normalized: subeditor)  | 4   
Mapping failed for 700 $e superivsing animator (Normalized: superivsing animator)  | 2   
Mapping failed for 700 $e supervising director. (Normalized: supervising director)  | 1   
Mapping failed for 700 $e supervising producer. (Normalized: supervising producer)  | 4   
Mapping failed for 700 $e t. aut. (Normalized: t aut)  | 1   
Mapping failed for 700 $e tech. cons. (Normalized: tech cons)  | 3   
Mapping failed for 700 $e tekst. (Normalized: tekst)  | 1   
Mapping failed for 700 $e television presenter. (Normalized: television presenter)  | 1   
Mapping failed for 700 $e televison producer. (Normalized: televison producer)  | 1   
Mapping failed for 700 $e text designer. (Normalized: text designer)  | 1   
Mapping failed for 700 $e text, ill. (Normalized: text ill)  | 1   
Mapping failed for 700 $e text. (Normalized: text)  | 3   
Mapping failed for 700 $e tr (Normalized: tr)  | 4   
Mapping failed for 700 $e tr. (Normalized: tr)  | 331   
Mapping failed for 700 $e tr., (Normalized: tr)  | 1   
Mapping failed for 700 $e tr.. (Normalized: tr)  | 1   
Mapping failed for 700 $e tra. (Normalized: tra)  | 7   
Mapping failed for 700 $e tran. (Normalized: tran)  | 2   
Mapping failed for 700 $e trans. (Normalized: trans)  | 207   
Mapping failed for 700 $e trans., adapt. (Normalized: trans adapt)  | 4   
Mapping failed for 700 $e trans., ed. (Normalized: trans ed)  | 1   
Mapping failed for 700 $e trans., interp. (Normalized: trans interp)  | 1   
Mapping failed for 700 $e trans., intro. (Normalized: trans intro)  | 1   
Mapping failed for 700 $e trans.3. (Normalized: trans3)  | 1   
Mapping failed for 700 $e translator of introduction. (Normalized: translator of introduction)  | 1   
Mapping failed for 700 $e translator.?UNAUTHORIZED (Normalized: translatorUNAUTHORIZED)  | 1   
Mapping failed for 700 $e translators. (Normalized: translators)  | 1   
Mapping failed for 700 $e trl (Normalized: trl)  | 1   
Mapping failed for 700 $e trl. (Normalized: trl)  | 34   
Mapping failed for 700 $e txt. (Normalized: txt)  | 1   
Mapping failed for 700 $e typography. (Normalized: typography)  | 1   
Mapping failed for 700 $e visual effects provider. (Normalized: visual effects provider)  | 2   
Mapping failed for 700 $e vocie actor. (Normalized: vocie actor)  | 1   
Mapping failed for 700 $e voiceovers. (Normalized: voiceovers)  | 2   
Mapping failed for 700 $e volume editor. (Normalized: volume editor)  | 1   
Mapping failed for 700 $e voz. (Normalized: voz)  | 2   
Mapping failed for 700 $e writer (Normalized: writer)  | 55   
Mapping failed for 700 $e writer , (Normalized: writer )  | 1   
Mapping failed for 700 $e writer and producer. (Normalized: writer and producer)  | 4   
Mapping failed for 700 $e writer of afterword. (Normalized: writer of afterword)  | 10   
Mapping failed for 700 $e writer of commentary. (Normalized: writer of commentary)  | 1   
Mapping failed for 700 $e writer of foreword (Normalized: writer of foreword)  | 3   
Mapping failed for 700 $e writer of foreword. (Normalized: writer of foreword)  | 32   
Mapping failed for 700 $e writer of introduction, etc. (Normalized: writer of introduction etc)  | 1   
Mapping failed for 700 $e writer of postface. (Normalized: writer of postface)  | 1   
Mapping failed for 700 $e writer of prelimiary note. (Normalized: writer of prelimiary note)  | 1   
Mapping failed for 700 $e writer of prologue. (Normalized: writer of prologue)  | 9   
Mapping failed for 700 $e writer of the introduction. (Normalized: writer of the introduction)  | 1   
Mapping failed for 700 $e writer,  (Normalized: writer)  | 1   
Mapping failed for 700 $e writer, (Normalized: writer)  | 17   
Mapping failed for 700 $e writer. (Normalized: writer)  | 130   
Mapping failed for 700 $e writing. (Normalized: writing)  | 2   
Mapping failed for 700 $e writter  (Normalized: writter)  | 1   
Mapping failed for 700 $e writter of preface. (Normalized: writter of preface)  | 1   
Mapping failed for 700 $e writter, (Normalized: writter)  | 2   
Mapping failed for 700 $e writter. (Normalized: writter)  | 5   
Mapping failed for 700 $e wrtier. (Normalized: wrtier)  | 1   
Mapping failed for 700 $e xecutive producer (Normalized: xecutive producer)  | 1   
Mapping failed for 700 $e xecutive producer , (Normalized: xecutive producer )  | 1   
Mapping failed for 700 $e xecutive producer ; (Normalized: xecutive producer )  | 1   
Mapping failed for 700 $e xecutive producer. (Normalized: xecutive producer)  | 30   
Mapping failed for 710 $e (Firm). (Normalized: Firm)  | 1   
Mapping failed for 710 $e (music band) (Normalized: music band)  | 1   
Mapping failed for 710 $e (music band). (Normalized: music band)  | 1   
Mapping failed for 710 $e Executive Producer. (Normalized: Executive Producer)  | 2   
Mapping failed for 710 $e Music band. (Normalized: Music band)  | 5   
Mapping failed for 710 $e associated with work. (Normalized: associated with work)  | 2   
Mapping failed for 710 $e colourist, (Normalized: colourist)  | 1   
Mapping failed for 710 $e colourist. (Normalized: colourist)  | 5   
Mapping failed for 710 $e comp. (Normalized: comp)  | 3   
Mapping failed for 710 $e composer (expression) (Normalized: composer expression)  | 1   
Mapping failed for 710 $e composer (expression), (Normalized: composer expression)  | 1   
Mapping failed for 710 $e consultants. (Normalized: consultants)  | 1   
Mapping failed for 710 $e contributing body. (Normalized: contributing body)  | 1   
Mapping failed for 710 $e corporate sponsor. (Normalized: corporate sponsor)  | 2   
Mapping failed for 710 $e designer and producer. (Normalized: designer and producer)  | 2   
Mapping failed for 710 $e distributer. (Normalized: distributer)  | 1   
Mapping failed for 710 $e distribution company. (Normalized: distribution company)  | 3   
Mapping failed for 710 $e ditor. (Normalized: ditor)  | 1   
Mapping failed for 710 $e ed. (Normalized: ed)  | 17   
Mapping failed for 710 $e editors. (Normalized: editors)  | 1   
Mapping failed for 710 $e executive producer ; (Normalized: executive producer )  | 1   
Mapping failed for 710 $e executive producer. (Normalized: executive producer)  | 4   
Mapping failed for 710 $e éd. (Normalized: ed)  | 1   
Mapping failed for 710 $e film distribuor. (Normalized: film distribuor)  | 1   
Mapping failed for 710 $e film presenter (Normalized: film presenter)  | 1   
Mapping failed for 710 $e film presenter. (Normalized: film presenter)  | 4   
Mapping failed for 710 $e film production company (Normalized: film production company)  | 1   
Mapping failed for 710 $e film production company, (Normalized: film production company)  | 5   
Mapping failed for 710 $e film production company. (Normalized: film production company)  | 25   
Mapping failed for 710 $e ill (Normalized: ill)  | 2   
Mapping failed for 710 $e ill. (Normalized: ill)  | 21   
Mapping failed for 710 $e interior illustrator (Normalized: interior illustrator)  | 1   
Mapping failed for 710 $e interior illustrator?UNAUTHORIZED (Normalized: interior illustratorUNAUTHORIZED)  | 1   
Mapping failed for 710 $e issuing agency. (Normalized: issuing agency)  | 1   
Mapping failed for 710 $e jt. aut. (Normalized: jt aut)  | 1   
Mapping failed for 710 $e jt. ed. (Normalized: jt ed)  | 1   
Mapping failed for 710 $e letterer. (Normalized: letterer)  | 1   
Mapping failed for 710 $e meeting. (Normalized: meeting)  | 1   
Mapping failed for 710 $e music production company. (Normalized: music production company)  | 1   
Mapping failed for 710 $e musicians (Normalized: musicians)  | 1   
Mapping failed for 710 $e musicians. (Normalized: musicians)  | 1   
Mapping failed for 710 $e perfomer. (Normalized: perfomer)  | 1   
Mapping failed for 710 $e presener. (Normalized: presener)  | 1   
Mapping failed for 710 $e producer ; (Normalized: producer )  | 1   
Mapping failed for 710 $e production company , (Normalized: production company )  | 1   
Mapping failed for 710 $e prodution company. (Normalized: prodution company)  | 1   
Mapping failed for 710 $e publishing body. (Normalized: publishing body)  | 1   
Mapping failed for 710 $e special effects. (Normalized: special effects)  | 1   
Mapping failed for 710 $e sponsoring body. (Normalized: sponsoring body)  | 7   
Mapping failed for 710 $e television production company. (Normalized: television production company)  | 2   
Mapping failed for 710 $e tr. (Normalized: tr)  | 2   
Mapping failed for 710 $e typesetter. (Normalized: typesetter)  | 1   
Mapping failed for 710 $e visual effects provider, (Normalized: visual effects provider)  | 1   
Mapping failed for 720 $e ill. (Normalized: ill)  | 3   
</details>   
   
## Mapped publisher role from Indicator2    
Publication Role, taken from the code in Ind2    
<details><summary>Click to expand all 11 things</summary>     
   
Measure | Count   
--- | ---:   
264 ind2  -> | 2,464   
264 ind2 0->Production | 116   
264 ind2 1->Publication | 24,425   
264 ind2 2->Distribution | 237   
264 ind2 3->Manufacture | 244   
264 ind2 4->Copyright notice date | 18,027   
264 ind2 5-> | 1   
264 ind2 6-> | 2   
264 ind2 7-> | 2   
880 ind2 1->Publication | 3   
</details>   
   
## Mapped electronic access relationships types    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Electronic access relationship type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 5 things</summary>     
   
Measure | Count   
--- | ---:   
No information provided | 21,733   
Related resource | 354   
Resource | 6,962   
Version of resource | 277   
</details>   
   
## Preceding and Succeeding titles    
    
<details><summary>Click to expand all 3 things</summary>     
   
Measure | Count   
--- | ---:   
precedingTitles created | 197   
succeedingTitles created | 83   
</details>   
   
## Holdings generation from bibs    
Some libraries have Holdings/MFHD information baked into their bib records. The following breakdown gives an idea on the occurrence of 852/866 combinations    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Records with both 852s and at least one 86X | 1,900   
</details>   
   
## Instance format ids handling (337 + 338))    
    
<details><summary>Click to expand all 68 things</summary>     
   
Measure | Count   
--- | ---:   
338$b is missing. Will try parse from 337$a and 338$a | 4,241   
Code 'dv' not found in FOLIO | 6   
Code from 338$b NOT found in FOLIO: "  " | 1   
Code from 338$b NOT found in FOLIO: " nc " | 5   
Code from 338$b NOT found in FOLIO: " nc" | 1   
Code from 338$b NOT found in FOLIO: "c " | 1   
Code from 338$b NOT found in FOLIO: "dv" | 6   
Code from 338$b NOT found in FOLIO: "n " | 5   
Code from 338$b NOT found in FOLIO: "n" | 7   
Code from 338$b NOT found in FOLIO: "nc " | 1   
Code from 338$b NOT found in FOLIO: "rdacarrier" | 2   
Code from 338$b NOT found in FOLIO: "s " | 1   
Code from 338$b NOT found in FOLIO: "s" | 1   
Code from 338$b NOT found in FOLIO: "tx" | 1   
Instance Format not mapped from field since 338$2 is missing | 34   
InstanceFormat not mapped since 338$2 (Source) is set to .  | 1   
InstanceFormat not mapped since 338$2 (Source) is set to carrier.  | 1   
InstanceFormat not mapped since 338$2 (Source) is set to nc.  | 1   
InstanceFormat not mapped since 338$2 (Source) is set to r dacarrier.  | 1   
InstanceFormat not mapped since 338$2 (Source) is set to radcarrier.  | 1   
InstanceFormat not mapped since 338$2 (Source) is set to rda carrier.  | 1   
InstanceFormat not mapped since 338$2 (Source) is set to rdacarreir.  | 6   
InstanceFormat not mapped since 338$2 (Source) is set to rdacontent.  | 19   
InstanceFormat not mapped since 338$2 (Source) is set to rdamedia.  | 11   
InstanceFormat not mapped since 338$2 (Source) is set to rdavolume.  | 1   
InstanceFormat not mapped since 338$2 (Source) is set to rdcarrier.  | 13   
Successful match  - "cd"->computer -- computer disc | 95   
Successful match  - "cr"->computer -- online resource | 6,945   
Successful match  - "mr"->projected image -- film reel | 1   
Successful match  - "nb"->unmediated -- sheet | 21   
Successful match  - "nc"->unmediated -- volume | 22,626   
Successful match  - "no"->unmediated -- card | 2   
Successful match  - "nr"->unmediated -- object | 37   
Successful match  - "nz"->unmediated -- other | 10   
Successful match  - "sd"->audio -- audio disc | 1,726   
Successful match  - "vc"->video -- video cartridge | 1   
Successful match  - "vd"->video -- videodisc | 660   
Successful match  - "vf"->video -- videocassette | 2   
Successful match  - "vz"->video -- other | 2   
Successful match  - cd->computer -- computer disc | 94   
Successful match  - cr->computer -- online resource | 6,945   
Successful match  - mr->projected image -- film reel | 1   
Successful match  - nb->unmediated -- sheet | 21   
Successful match  - nc->unmediated -- volume | 22,575   
Successful match  - nn->unmediated -- flipchart | 7   
Successful match  - no->unmediated -- card | 2   
Successful match  - nr->unmediated -- object | 37   
Successful match  - nz->unmediated -- other | 10   
Successful match  - sd->audio -- audio disc | 1,726   
Successful match  - ss->audio -- audiocassette | 2   
Successful match  - vc->video -- video cartridge | 1   
Successful match  - vd->video -- videodisc | 659   
Successful match  - vf->video -- videocassette | 2   
Successful match  - vz->video -- other | 2   
Successful matching on 337$a & 338$a - audio -- audio disc->audio -- audio disc | 20   
Successful matching on 337$a & 338$a - computer -- computer disc->computer -- computer disc | 18   
Successful matching on 337$a & 338$a - computer -- online resource->computer -- online resource | 1   
Successful matching on 337$a & 338$a - unmediated -- object->unmediated -- object | 1   
Successful matching on 337$a & 338$a - unmediated -- sheet->unmediated -- sheet | 1   
Successful matching on 337$a & 338$a - unmediated -- volume->unmediated -- volume | 4,172   
Successful matching on 337$a & 338$a - video -- videodisc->video -- videodisc | 16   
Unsuccessful matching on 337$a and 338$a - audio -- audiodisc | 1   
Unsuccessful matching on 337$a and 338$a - two-dimensional moving image -- volume | 1   
Unsuccessful matching on 337$a and 338$a - unmdiated -- volume | 2   
Unsuccessful matching on 337$a and 338$a - unmediate -- volume | 1   
Unsuccessful matching on 337$a and 338$a - unmediated -- computer disc | 1   
Unsuccessful matching on 337$a and 338$a - unmedited -- volume | 4   
</details>   
   
## Resource Type Mapping (336)    
Library action: **REVIEW** <br/>The created FOLIO instances contain the following Instance type values. The library should review the total number for each value against what they would expect to see mapped.    
<details><summary>Click to expand all 39 things</summary>     
   
Measure | Count   
--- | ---:   
336$a - Successful matching on  cartographicimage (cartographic image) | 4   
336$a - Successful matching on  computerprogram (computer program) | 1   
336$a - Successful matching on  notatedmusic (notated music) | 3   
336$a - Successful matching on  performedmusic (performed music) | 3   
336$a - Successful matching on  spokenword (spoken word) | 12   
336$a - Successful matching on  stillimage (still image) | 7   
336$a - Successful matching on  text (Text) | 1   
336$a - Successful matching on  text (text) | 4,179   
336$a - Successful matching on  two-dimensionalmovingimage (two-dimensional moving image) | 14   
336$a - Unsuccessful matching on   () | 6   
336$a - Unsuccessful matching on  atext$2rdacontent ( a text $2 rdacontent) | 1   
336$a - Unsuccessful matching on  rdacontent (rdacontent) | 1   
336$a - Unsuccessful matching on  texttxtrdacontent (text txt rdacontent) | 7   
336$a - Unsuccessful matching on  tezxt (tezxt) | 1   
336$a - Unsuccessful matching on  txt (txt) | 2   
336$b - Code  ('') not found in FOLIO  | 1   
336$b - Code rdacontent ('rdacontent') not found in FOLIO  | 2   
336$b - Code t ('t') not found in FOLIO  | 1   
336$b - Code tx ('tx') not found in FOLIO  | 2   
336$b cartographic image mapped from cri | 13   
336$b computer program mapped from cop | 1   
336$b notated music mapped from ntm | 31   
336$b other mapped from xxx | 2   
336$b performed music mapped from prm | 173   
336$b sounds mapped from snd | 2   
336$b spoken word mapped from spw | 1,729   
336$b still image mapped from sti | 103   
336$b tactile image mapped from tci | 1   
336$b tactile text mapped from tct | 11   
336$b tactile three-dimensional form mapped from tcf | 2   
336$b text mapped from  txt | 4   
336$b text mapped from  txt  | 4   
336$b text mapped from txt | 29,266   
336$b text mapped from txt  | 1   
336$b three-dimensional form mapped from tdf | 31   
336$b three-dimensional moving image mapped from tdm | 8   
336$b two-dimensional moving image mapped from tdi | 649   
Subfield b not in 336 | 4,244   
</details>   
   
## Incomplete entity mapping adding entity    
**NO ACTION REQUIRED** <br/>This is a coding anomaly that FSE will look into.  <br/>Usually, the library does not have to do anything about it.<br/> One thing to look at is if there are many repeated subfields or unexpected patterns of subfields in the table.    
<details><summary>Click to expand all 29 things</summary>     
   
Measure | Count   
--- | ---:   
024 a:empty ->>-->> identifiers    | 6   
024 z:has_value - d:has_value ->>-->> identifiers    | 2   
024 z:has_value - q:has_value ->>-->> identifiers    | 2   
024 z:has_value ->>-->> identifiers    | 54   
028 a:empty ->>-->> identifiers    | 3   
082 2:has_value ->>-->> classifications    | 4   
082 R:has_value - 2:has_value ->>-->> classifications    | 1   
082 a:empty ->>-->> classifications    | 19   
090 a:empty ->>-->> classifications    | 2   
100 a:empty ->>-->> contributors    | 4   
110 a:empty ->>-->> contributors    | 1   
600 a:empty ->>-->> subjects    | 1   
650 a:empty ->>-->> subjects    | 7   
650 a:has_value ->>-->> subjects    | 1   
651 a:empty ->>-->> subjects    | 4   
655 2:has_value ->>-->> subjects    | 1   
655 a:empty ->>-->> subjects    | 2   
700 a:empty ->>-->> contributors    | 3   
710 a:empty ->>-->> contributors    | 1   
800 a:empty ->>-->> series    | 2   
830 a:empty ->>-->> series    | 2   
856 3:has_value ->>-->> electronicAccess    | 1   
856 a:has_value - 2:has_value ->>-->> electronicAccess    | 3   
856 a:has_value - c:has_value - f:has_value - n:has_value - o:has_value - q:has_value - s:has_value ->>-->> electronicAccess    | 1   
856 a:has_value - z:has_value - x:has_value ->>-->> electronicAccess    | 1   
856 a:has_value ->>-->> electronicAccess    | 12   
856 h:has_value - 2:has_value ->>-->> electronicAccess    | 1   
856 z:has_value ->>-->> electronicAccess    | 1   
</details>   
   
## Unrecognized language codes in records    
Library action: **REVIEW** <br/>Language code values in the source data that do not match standard language codes. If not fixed before migration, these will display as Undetermined in the instance record and Filtering by language in Inventory will not be conclusive.    
<details><summary>Click to expand all 33 things</summary>     
   
Measure | Count   
--- | ---:   
Unrecognized language codes in record:   g | 1   
Unrecognized language codes in record:  eg | 1   
Unrecognized language codes in record:  en | 3   
Unrecognized language codes in record: +ng | 1   
Unrecognized language codes in record: and | 4   
Unrecognized language codes in record: arb | 1   
Unrecognized language codes in record: can | 1   
Unrecognized language codes in record: d   | 6   
Unrecognized language codes in record: ebg | 1   
Unrecognized language codes in record: emg | 2   
Unrecognized language codes in record: emn | 2   
Unrecognized language codes in record: en0 | 1   
Unrecognized language codes in record: end | 5   
Unrecognized language codes in record: enf | 10   
Unrecognized language codes in record: enh | 2   
Unrecognized language codes in record: enk | 78   
Unrecognized language codes in record: enn | 5   
Unrecognized language codes in record: ent | 3   
Unrecognized language codes in record: fr  | 3   
Unrecognized language codes in record: geb | 1   
Unrecognized language codes in record: hih | 1   
Unrecognized language codes in record: jpa | 1   
Unrecognized language codes in record: kri | 1   
Unrecognized language codes in record: mri | 1   
Unrecognized language codes in record: n94 | 1   
Unrecognized language codes in record: pcc | 1   
Unrecognized language codes in record: ren | 1   
Unrecognized language codes in record: sap | 1   
Unrecognized language codes in record: sng | 1   
Unrecognized language codes in record: sp  | 2   
Unrecognized language codes in record: tne | 1   
Unrecognized language codes in record: |   | 2   
</details>   
   
## Leader manipulation    
    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
Set leader 20-23 from 45 0 to 4500 | 2,437   
</details>   
   
## 880 mappings    
This table shows how the 880 (Alternate Graphic Representation) has been mapped.    
<details><summary>Click to expand all 113 things</summary>     
   
Measure | Count   
--- | ---:   
Mapping not set up for target field: 440 (440-03/$1) | 1   
Mapping not set up for target field: 490 (490-00/$1) | 3   
Mapping not set up for target field: 490 (490-03/$1) | 4   
Mapping not set up for target field: 490 (490-04) | 2   
Mapping not set up for target field: 490 (490-04/$1) | 14   
Mapping not set up for target field: 490 (490-05/$1) | 3   
Mapping not set up for target field: 490 (490-06/$1) | 1   
Mapping not set up for target field: 490 (490-08/$1) | 2   
Mapping not set up for target field: 658 (658-00) | 1   
Mapping not set up for target field: 730 (730-08/$1) | 1   
Mapping not set up for target field: 765 (765-00/(3/r) | 1   
Mapping not set up for target field: 787 (787-00) | 1   
Records without $6 | 1   
Source digits: 100-01/$1 Target field: 700 | 17   
Source digits: 100-01/(3/r Target field: 700 | 1   
Source digits: 130-01/$1 Target field: 130 | 4   
Source digits: 240-00 Target field: 240 | 2   
Source digits: 240-00/$1 Target field: 240 | 1   
Source digits: 240-00/(3/r Target field: 240 | 1   
Source digits: 240-01/$1 Target field: 240 | 2   
Source digits: 240-02/$1 Target field: 240 | 13   
Source digits: 245-01 Target field: 246 | 3   
Source digits: 245-01/$1 Target field: 246 | 32   
Source digits: 245-02/$1 Target field: 246 | 6   
Source digits: 245-03/$1 Target field: 246 | 3   
Source digits: 246-00/$1 Target field: 246 | 3   
Source digits: 246-01/$1 Target field: 246 | 2   
Source digits: 246-02/$1 Target field: 246 | 4   
Source digits: 246-03/$1 Target field: 246 | 4   
Source digits: 246-04/$1 Target field: 246 | 1   
Source digits: 246-05/$1 Target field: 246 | 1   
Source digits: 250-00/$1 Target field: 250 | 1   
Source digits: 250-02 Target field: 250 | 3   
Source digits: 250-02/$1 Target field: 250 | 19   
Source digits: 250-03/$1 Target field: 250 | 4   
Source digits: 250-04/$1 Target field: 250 | 4   
Source digits: 250-06/$1 Target field: 250 | 1   
Source digits: 260-00 Target field: 260 | 1   
Source digits: 260-00/$1 Target field: 260 | 3   
Source digits: 260-02/$1 Target field: 260 | 6   
Source digits: 260-03 Target field: 260 | 3   
Source digits: 260-03/$1 Target field: 260 | 18   
Source digits: 260-04/$1 Target field: 260 | 4   
Source digits: 260-05/$1 Target field: 260 | 4   
Source digits: 260-07/$1 Target field: 260 | 1   
Source digits: 264-00 Target field: 264 | 1   
Source digits: 264-03/$1 Target field: 264 | 2   
Source digits: 300-00/$1 Target field: 300 | 1   
Source digits: 362-03/$1 Target field: 362 | 1   
Source digits: 440-03/$1 Target field: 440 | 1   
Source digits: 490-00/$1 Target field: 490 | 3   
Source digits: 490-03/$1 Target field: 490 | 4   
Source digits: 490-04 Target field: 490 | 2   
Source digits: 490-04/$1 Target field: 490 | 14   
Source digits: 490-05/$1 Target field: 490 | 3   
Source digits: 490-06/$1 Target field: 490 | 1   
Source digits: 490-08/$1 Target field: 490 | 2   
Source digits: 500-00 Target field: 500 | 5   
Source digits: 500-00/$1 Target field: 500 | 3   
Source digits: 500-02/(3/r Target field: 500 | 1   
Source digits: 500-03/$1 Target field: 500 | 1   
Source digits: 500-04/$1 Target field: 500 | 2   
Source digits: 500-05/$1 Target field: 500 | 1   
Source digits: 505-00/$1 Target field: 505 | 1   
Source digits: 505-04/$1 Target field: 505 | 1   
Source digits: 520-00 Target field: 520 | 1   
Source digits: 520-00/$1 Target field: 520 | 1   
Source digits: 600-00 Target field: 600 | 2   
Source digits: 600-03/$1 Target field: 600 | 2   
Source digits: 600-07 Target field: 600 | 1   
Source digits: 610-04/$1 Target field: 610 | 2   
Source digits: 610-05/$1 Target field: 610 | 1   
Source digits: 650-00 Target field: 650 | 1   
Source digits: 650-00/$1 Target field: 650 | 2   
Source digits: 650-03/$1 Target field: 650 | 1   
Source digits: 650-04/$1 Target field: 650 | 2   
Source digits: 650-05/$1 Target field: 650 | 2   
Source digits: 650-06/$1 Target field: 650 | 1   
Source digits: 651-05/$1 Target field: 651 | 2   
Source digits: 658-00 Target field: 658 | 1   
Source digits: 700-00/$1 Target field: 700 | 6   
Source digits: 700-00/(2/r Target field: 700 | 1   
Source digits: 700-01/$1 Target field: 700 | 1   
Source digits: 700-02/$1 Target field: 700 | 1   
Source digits: 700-03/$1 Target field: 700 | 2   
Source digits: 700-04 Target field: 700 | 1   
Source digits: 700-04/$1 Target field: 700 | 7   
Source digits: 700-05 Target field: 700 | 1   
Source digits: 700-05/$1 Target field: 700 | 13   
Source digits: 700-06 Target field: 700 | 1   
Source digits: 700-06/$1 Target field: 700 | 5   
Source digits: 700-07/$1 Target field: 700 | 3   
Source digits: 700-09/$1 Target field: 700 | 1   
Source digits: 710-00 Target field: 710 | 1   
Source digits: 710-00/$1 Target field: 710 | 1   
Source digits: 710-02/$1 Target field: 710 | 4   
Source digits: 710-04/$1 Target field: 710 | 3   
Source digits: 710-05/$1 Target field: 710 | 4   
Source digits: 710-06/$1 Target field: 710 | 6   
Source digits: 710-07/$1 Target field: 710 | 4   
Source digits: 730-08/$1 Target field: 730 | 1   
Source digits: 765-00/(3/r Target field: 765 | 1   
Source digits: 787-00 Target field: 787 | 1   
Source digits: 830-05 Target field: 830 | 1   
Source digits: 830-05/$1 Target field: 830 | 1   
Source digits: 830-06/$1 Target field: 830 | 9   
Source digits: 830-07 Target field: 830 | 1   
Source digits: 830-07/$1 Target field: 830 | 4   
Source digits: 830-08/$1 Target field: 830 | 3   
Source digits: 830-09/$1 Target field: 830 | 2   
Source digits: 830-10/$1 Target field: 830 | 1   
Source digits: 830-97/$1 Target field: 830 | 1   
</details>   
   
## Set note to staff only via indicator    
    
<details><summary>Click to expand all 7 things</summary>     
   
Measure | Count   
--- | ---:   
541 indicator1:   (1 is public, all other values are Staff only) | 13   
541 indicator1: 1 (1 is public, all other values are Staff only) | 4   
542 indicator1:   (1 is public, all other values are Staff only) | 6   
561 indicator1:   (1 is public, all other values are Staff only) | 2   
583 indicator1:   (1 is public, all other values are Staff only) | 8   
583 indicator1: 1 (1 is public, all other values are Staff only) | 3   
</details>   
   
## Language code sources in 041    
Most language codes in MARC records come from this list: https://www.loc.gov/marc/languages/, But other codes are allowed. The controlled vocabulary needs to be stated in $2 and this is where the information in this list comes from. The mapping tools can not currently handle other language codes, and so cannot FOLIO. <br/>One solution is to migrate the codes into a string or/and replace the language code with the parent language (these languages are usually subgroups of other languages). Many times, these records already have the "super-language" recorded as well. The data will remain in the MARC records.    
<details><summary>Click to expand all 2 things</summary>     
   
Measure | Count   
--- | ---:   
iso639-3 | 1   
</details>   

## Mapped FOLIO fields
<details><summary>Click to expand field report</summary>     

FOLIO Field | Mapped | Unmapped  
--- | --- | ---:  
_version | 0 (0%) | 162,983 (100%) 
administrativeNotes | 162,979 (100%) | 4 (0%) 
alternativeTitles | 25,671 (16%) | 137,312 (84%) 
alternativeTitles.alternativeTitle | 25,653 (16%) | 137,330 (84%) 
alternativeTitles.alternativeTitleTypeId | 25,671 (16%) | 137,312 (84%) 
catalogedDate | 0 (0%) | 162,983 (100%) 
classifications | 56,417 (35%) | 106,566 (65%) 
classifications.classificationNumber | 56,417 (35%) | 106,566 (65%) 
classifications.classificationTypeId | 56,417 (35%) | 106,566 (65%) 
contributors | 158,755 (97%) | 4,228 (3%) 
contributors.contributorNameTypeId | 158,755 (97%) | 4,228 (3%) 
contributors.contributorTypeId | 20,561 (13%) | 142,422 (87%) 
contributors.contributorTypeText | 21,595 (13%) | 141,388 (87%) 
contributors.name | 158,755 (97%) | 4,228 (3%) 
contributors.primary | 141,489 (87%) | 21,494 (13%) 
discoverySuppress | 162,979 (100%) | 4 (0%) 
editions | 41,199 (25%) | 121,784 (75%) 
electronicAccess | 8,214 (5%) | 154,769 (95%) 
electronicAccess.linkText | 3 (0%) | 162,980 (100%) 
electronicAccess.materialsSpecification | 8,106 (5%) | 154,877 (95%) 
electronicAccess.publicNote | 6,957 (4%) | 156,026 (96%) 
electronicAccess.relationshipId | 8,214 (5%) | 154,769 (95%) 
electronicAccess.uri | 8,214 (5%) | 154,769 (95%) 
holdingsRecords2 | 0 (0%) | 162,983 (100%) 
hrid | 162,979 (100%) | 4 (0%) 
id | 162,979 (100%) | 4 (0%) 
identifiers | 162,979 (100%) | 4 (0%) 
identifiers.identifierTypeId | 162,979 (100%) | 4 (0%) 
identifiers.value | 162,979 (100%) | 4 (0%) 
indexTitle | 162,975 (100%) | 8 (0%) 
instanceFormatIds | 162,979 (100%) | 4 (0%) 
instanceFormats | 0 (0%) | 162,983 (100%) 
instanceTypeId | 162,979 (100%) | 4 (0%) 
languages | 162,979 (100%) | 4 (0%) 
matchKey | 0 (0%) | 162,983 (100%) 
metadata | 162,979 (100%) | 4 (0%) 
metadata.createdByUserId | 162,979 (100%) | 4 (0%) 
metadata.createdDate | 162,979 (100%) | 4 (0%) 
metadata.updatedByUserId | 162,979 (100%) | 4 (0%) 
metadata.updatedDate | 162,979 (100%) | 4 (0%) 
modeOfIssuanceId | 162,979 (100%) | 4 (0%) 
natureOfContentTermIds | 0 (0%) | 162,983 (100%) 
notes | 127,960 (79%) | 35,023 (21%) 
notes.instanceNoteTypeId | 127,960 (79%) | 35,023 (21%) 
notes.note | 127,957 (79%) | 35,026 (21%) 
notes.staffOnly | 33 (0%) | 162,950 (100%) 
physicalDescriptions | 161,532 (99%) | 1,451 (1%) 
previouslyHeld | 0 (0%) | 162,983 (100%) 
publication | 161,630 (99%) | 1,353 (1%) 
publication.dateOfPublication | 160,464 (98%) | 2,519 (2%) 
publication.place | 158,985 (98%) | 3,998 (2%) 
publication.publisher | 158,768 (97%) | 4,215 (3%) 
publication.role | 24,865 (15%) | 138,118 (85%) 
publicationFrequency | 818 (1%) | 162,165 (99%) 
publicationPeriod | 0 (0%) | 162,983 (100%) 
publicationRange | 838 (1%) | 162,145 (99%) 
series | 27,467 (17%) | 135,516 (83%) 
series.value | 27,467 (17%) | 135,516 (83%) 
source | 162,979 (100%) | 4 (0%) 
sourceRecordFormat | 0 (0%) | 162,983 (100%) 
staffSuppress | 162,979 (100%) | 4 (0%) 
statisticalCodeIds | 0 (0%) | 162,983 (100%) 
statusId | 0 (0%) | 162,983 (100%) 
statusUpdatedDate | 0 (0%) | 162,983 (100%) 
subjects | 148,095 (91%) | 14,888 (9%) 
subjects.value | 148,095 (91%) | 14,888 (9%) 
tags | 0 (0%) | 162,983 (100%) 
title | 162,979 (100%) | 4 (0%) 
</details>   

## Mapped Legacy fields
<details><summary>Click to expand field report</summary>     

Legacy Field | Present | Mapped | Unmapped  
--- | --- | --- | ---:  
001 | 162,983 (100.0%) | 162,983 (100%) | 0  
003 | 162,986 (100.0%) | 0 (0%) | 162,986  
004 | 3 (0.0%) | 0 (0%) | 3  
005 | 152,636 (93.7%) | 0 (0%) | 152,636  
006 | 7,439 (4.6%) | 0 (0%) | 7,439  
007 | 12,403 (7.6%) | 0 (0%) | 12,403  
008 | 162,983 (100.0%) | 162,983 (100%) | 0  
009 | 1 (0.0%) | 0 (0%) | 1  
010 | 82,085 (50.4%) | 82,085 (50%) | 0  
011 | 2 (0.0%) | 0 (0%) | 2  
012 | 88 (0.1%) | 0 (0%) | 88  
015 | 12,571 (7.7%) | 0 (0%) | 12,571  
016 | 2,076 (1.3%) | 0 (0%) | 2,076  
017 | 63 (0.0%) | 0 (0%) | 63  
018 | 1 (0.0%) | 0 (0%) | 1  
019 | 5,245 (3.2%) | 5,245 (3%) | 0  
020 | 214,546 (131.6%) | 214,546 (132%) | 0  
021 | 3 (0.0%) | 0 (0%) | 3  
022 | 368 (0.2%) | 368 (0%) | 0  
024 | 2,583 (1.6%) | 2,583 (2%) | 0  
025 | 153 (0.1%) | 0 (0%) | 153  
028 | 3,834 (2.4%) | 3,834 (2%) | 0  
029 | 1,817 (1.1%) | 0 (0%) | 1,817  
030 | 21 (0.0%) | 0 (0%) | 21  
031 | 7 (0.0%) | 0 (0%) | 7  
032 | 34 (0.0%) | 0 (0%) | 34  
033 | 49 (0.0%) | 0 (0%) | 49  
034 | 96 (0.1%) | 0 (0%) | 96  
035 | 215,584 (132.3%) | 215,584 (132%) | 0  
037 | 9,082 (5.6%) | 0 (0%) | 9,082  
038 | 1 (0.0%) | 0 (0%) | 1  
039 | 274 (0.2%) | 0 (0%) | 274  
040 | 144,862 (88.9%) | 0 (0%) | 144,862  
041 | 6,385 (3.9%) | 6,385 (4%) | 0  
042 | 38,788 (23.8%) | 0 (0%) | 38,788  
043 | 32,693 (20.1%) | 0 (0%) | 32,693  
044 | 62 (0.0%) | 0 (0%) | 62  
045 | 56 (0.0%) | 0 (0%) | 56  
046 | 131 (0.1%) | 0 (0%) | 131  
047 | 15 (0.0%) | 0 (0%) | 15  
048 | 40 (0.0%) | 0 (0%) | 40  
049 | 88,104 (54.1%) | 0 (0%) | 88,104  
050 | 42,720 (26.2%) | 42,720 (26%) | 0  
051 | 90 (0.1%) | 0 (0%) | 90  
052 | 100 (0.1%) | 0 (0%) | 100  
055 | 1,612 (1.0%) | 0 (0%) | 1,612  
060 | 510 (0.3%) | 510 (0%) | 0  
066 | 218 (0.1%) | 0 (0%) | 218  
069 | 119 (0.1%) | 0 (0%) | 119  
070 | 88 (0.1%) | 0 (0%) | 88  
072 | 120 (0.1%) | 0 (0%) | 120  
074 | 5 (0.0%) | 5 (0%) | 0  
079 | 1 (0.0%) | 0 (0%) | 1  
080 | 21 (0.0%) | 21 (0%) | 0  
082 | 21,221 (13.0%) | 21,221 (13%) | 0  
083 | 1 (0.0%) | 0 (0%) | 1  
084 | 6,981 (4.3%) | 0 (0%) | 6,981  
086 | 15 (0.0%) | 15 (0%) | 0  
088 | 5 (0.0%) | 0 (0%) | 5  
089 | 3 (0.0%) | 0 (0%) | 3  
090 | 3,845 (2.4%) | 3,845 (2%) | 0  
092 | 134,615 (82.6%) | 0 (0%) | 134,615  
093 | 1 (0.0%) | 0 (0%) | 1  
094 | 5 (0.0%) | 0 (0%) | 5  
095 | 2 (0.0%) | 0 (0%) | 2  
096 | 88 (0.1%) | 0 (0%) | 88  
097 | 8 (0.0%) | 0 (0%) | 8  
098 | 116 (0.1%) | 0 (0%) | 116  
099 | 18 (0.0%) | 0 (0%) | 18  
100 | 137,660 (84.5%) | 137,660 (84%) | 0  
110 | 3,609 (2.2%) | 3,609 (2%) | 0  
111 | 236 (0.1%) | 236 (0%) | 0  
130 | 872 (0.5%) | 872 (1%) | 0  
200 | 2 (0.0%) | 0 (0%) | 2  
210 | 142 (0.1%) | 0 (0%) | 142  
212 | 1 (0.0%) | 0 (0%) | 1  
222 | 178 (0.1%) | 0 (0%) | 178  
240 | 4,528 (2.8%) | 4,528 (3%) | 0  
242 | 64 (0.0%) | 0 (0%) | 64  
243 | 9 (0.0%) | 0 (0%) | 9  
245 | 163,018 (100.0%) | 163,018 (100%) | 0  
246 | 26,486 (16.3%) | 26,486 (16%) | 0  
247 | 4 (0.0%) | 4 (0%) | 0  
249 | 10 (0.0%) | 0 (0%) | 10  
250 | 41,274 (25.3%) | 41,274 (25%) | 0  
254 | 2 (0.0%) | 0 (0%) | 2  
255 | 121 (0.1%) | 121 (0%) | 0  
256 | 36 (0.0%) | 0 (0%) | 36  
257 | 236 (0.1%) | 0 (0%) | 236  
259 | 1 (0.0%) | 0 (0%) | 1  
260 | 135,415 (83.1%) | 135,415 (83%) | 0  
261 | 2 (0.0%) | 0 (0%) | 2  
263 | 648 (0.4%) | 0 (0%) | 648  
264 | 45,518 (27.9%) | 45,518 (28%) | 0  
265 | 39 (0.0%) | 0 (0%) | 39  
270 | 1,508 (0.9%) | 0 (0%) | 1,508  
300 | 161,619 (99.2%) | 161,619 (99%) | 0  
302 | 2 (0.0%) | 0 (0%) | 2  
306 | 2,203 (1.4%) | 0 (0%) | 2,203  
310 | 818 (0.5%) | 818 (1%) | 0  
321 | 94 (0.1%) | 94 (0%) | 0  
330 | 1 (0.0%) | 0 (0%) | 1  
336 | 41,164 (25.3%) | 36,281 (22%) | 4,883  
337 | 36,730 (22.5%) | 0 (0%) | 36,730  
338 | 36,425 (22.3%) | 36,425 (22%) | 0  
340 | 329 (0.2%) | 0 (0%) | 329  
341 | 1 (0.0%) | 0 (0%) | 1  
344 | 2,536 (1.6%) | 0 (0%) | 2,536  
345 | 81 (0.0%) | 0 (0%) | 81  
346 | 419 (0.3%) | 0 (0%) | 419  
347 | 2,582 (1.6%) | 0 (0%) | 2,582  
350 | 388 (0.2%) | 0 (0%) | 388  
362 | 856 (0.5%) | 856 (1%) | 0  
365 | 3 (0.0%) | 0 (0%) | 3  
366 | 5 (0.0%) | 0 (0%) | 5  
380 | 404 (0.2%) | 0 (0%) | 404  
381 | 2 (0.0%) | 0 (0%) | 2  
382 | 1 (0.0%) | 0 (0%) | 1  
385 | 34 (0.0%) | 0 (0%) | 34  
386 | 22 (0.0%) | 0 (0%) | 22  
390 | 1 (0.0%) | 0 (0%) | 1  
400 | 6 (0.0%) | 0 (0%) | 6  
410 | 3 (0.0%) | 0 (0%) | 3  
440 | 23,663 (14.5%) | 0 (0%) | 23,663  
449 | 1 (0.0%) | 0 (0%) | 1  
490 | 38,809 (23.8%) | 0 (0%) | 38,809  
491 | 1 (0.0%) | 0 (0%) | 1  
492 | 1 (0.0%) | 0 (0%) | 1  
499 | 1 (0.0%) | 0 (0%) | 1  
500 | 103,230 (63.3%) | 103,230 (63%) | 0  
501 | 33 (0.0%) | 33 (0%) | 0  
502 | 54 (0.0%) | 54 (0%) | 0  
503 | 2 (0.0%) | 0 (0%) | 2  
504 | 43,226 (26.5%) | 43,226 (27%) | 0  
505 | 25,728 (15.8%) | 25,728 (16%) | 0  
506 | 56 (0.0%) | 56 (0%) | 0  
507 | 1 (0.0%) | 1 (0%) | 0  
508 | 3,068 (1.9%) | 3,068 (2%) | 0  
510 | 225 (0.1%) | 225 (0%) | 0  
511 | 4,223 (2.6%) | 4,223 (3%) | 0  
513 | 2 (0.0%) | 2 (0%) | 0  
515 | 116 (0.1%) | 116 (0%) | 0  
516 | 5 (0.0%) | 5 (0%) | 0  
518 | 214 (0.1%) | 214 (0%) | 0  
520 | 66,361 (40.7%) | 66,361 (41%) | 0  
521 | 14,774 (9.1%) | 14,774 (9%) | 0  
522 | 1 (0.0%) | 1 (0%) | 0  
525 | 88 (0.1%) | 88 (0%) | 0  
526 | 1,581 (1.0%) | 1,581 (1%) | 0  
530 | 502 (0.3%) | 502 (0%) | 0  
533 | 2,120 (1.3%) | 2,120 (1%) | 0  
534 | 40 (0.0%) | 40 (0%) | 0  
535 | 2 (0.0%) | 2 (0%) | 0  
536 | 22 (0.0%) | 22 (0%) | 0  
538 | 6,815 (4.2%) | 6,815 (4%) | 0  
539 | 3 (0.0%) | 0 (0%) | 3  
540 | 189 (0.1%) | 189 (0%) | 0  
541 | 17 (0.0%) | 17 (0%) | 0  
542 | 6 (0.0%) | 6 (0%) | 0  
544 | 1 (0.0%) | 1 (0%) | 0  
545 | 95 (0.1%) | 95 (0%) | 0  
546 | 3,752 (2.3%) | 3,752 (2%) | 0  
547 | 2 (0.0%) | 2 (0%) | 0  
550 | 115 (0.1%) | 115 (0%) | 0  
555 | 28 (0.0%) | 28 (0%) | 0  
556 | 1 (0.0%) | 1 (0%) | 0  
561 | 2 (0.0%) | 2 (0%) | 0  
562 | 2 (0.0%) | 2 (0%) | 0  
563 | 2 (0.0%) | 2 (0%) | 0  
570 | 1 (0.0%) | 0 (0%) | 1  
580 | 84 (0.1%) | 84 (0%) | 0  
583 | 11 (0.0%) | 11 (0%) | 0  
586 | 1,376 (0.8%) | 1,376 (1%) | 0  
588 | 251 (0.2%) | 251 (0%) | 0  
592 | 25 (0.0%) | 0 (0%) | 25  
600 | 18,213 (11.2%) | 18,213 (11%) | 0  
605 | 1 (0.0%) | 0 (0%) | 1  
610 | 4,653 (2.9%) | 4,653 (3%) | 0  
611 | 296 (0.2%) | 296 (0%) | 0  
630 | 1,810 (1.1%) | 1,810 (1%) | 0  
647 | 24 (0.0%) | 24 (0%) | 0  
648 | 310 (0.2%) | 310 (0%) | 0  
650 | 395,119 (242.4%) | 395,119 (242%) | 0  
651 | 41,529 (25.5%) | 41,529 (25%) | 0  
653 | 2,946 (1.8%) | 0 (0%) | 2,946  
654 | 3 (0.0%) | 0 (0%) | 3  
655 | 63,718 (39.1%) | 63,718 (39%) | 0  
656 | 2 (0.0%) | 0 (0%) | 2  
657 | 2 (0.0%) | 0 (0%) | 2  
658 | 1 (0.0%) | 0 (0%) | 1  
659 | 1 (0.0%) | 0 (0%) | 1  
665 | 1 (0.0%) | 0 (0%) | 1  
675 | 1 (0.0%) | 0 (0%) | 1  
699 | 3 (0.0%) | 0 (0%) | 3  
700 | 96,636 (59.3%) | 96,636 (59%) | 0  
710 | 15,497 (9.5%) | 15,497 (10%) | 0  
711 | 270 (0.2%) | 270 (0%) | 0  
720 | 75 (0.0%) | 75 (0%) | 0  
730 | 2,647 (1.6%) | 0 (0%) | 2,647  
740 | 4,040 (2.5%) | 0 (0%) | 4,040  
750 | 1 (0.0%) | 0 (0%) | 1  
752 | 23 (0.0%) | 0 (0%) | 23  
753 | 56 (0.0%) | 0 (0%) | 56  
760 | 8 (0.0%) | 0 (0%) | 8  
765 | 6 (0.0%) | 0 (0%) | 6  
770 | 23 (0.0%) | 0 (0%) | 23  
772 | 7 (0.0%) | 0 (0%) | 7  
773 | 10 (0.0%) | 0 (0%) | 10  
774 | 12 (0.0%) | 0 (0%) | 12  
775 | 86 (0.1%) | 0 (0%) | 86  
776 | 2,436 (1.5%) | 0 (0%) | 2,436  
777 | 2 (0.0%) | 0 (0%) | 2  
780 | 197 (0.1%) | 197 (0%) | 0  
785 | 83 (0.1%) | 83 (0%) | 0  
786 | 1 (0.0%) | 0 (0%) | 1  
787 | 35 (0.0%) | 0 (0%) | 35  
791 | 1 (0.0%) | 0 (0%) | 1  
792 | 1 (0.0%) | 0 (0%) | 1  
800 | 11,244 (6.9%) | 11,244 (7%) | 0  
810 | 106 (0.1%) | 106 (0%) | 0  
811 | 4 (0.0%) | 4 (0%) | 0  
830 | 18,211 (11.2%) | 18,211 (11%) | 0  
840 | 4 (0.0%) | 0 (0%) | 4  
850 | 180 (0.1%) | 0 (0%) | 180  
852 | 1,987 (1.2%) | 0 (0%) | 1,987  
853 | 39 (0.0%) | 0 (0%) | 39  
856 | 29,326 (18.0%) | 29,326 (18%) | 0  
859 | 26 (0.0%) | 0 (0%) | 26  
863 | 39 (0.0%) | 0 (0%) | 39  
880 | 337 (0.2%) | 337 (0%) | 0  
886 | 70 (0.0%) | 0 (0%) | 70  
890 | 21 (0.0%) | 0 (0%) | 21  
891 | 8 (0.0%) | 0 (0%) | 8  
900 | 30 (0.0%) | 0 (0%) | 30  
901 | 13 (0.0%) | 0 (0%) | 13  
904 | 1 (0.0%) | 0 (0%) | 1  
905 | 1 (0.0%) | 0 (0%) | 1  
906 | 161 (0.1%) | 0 (0%) | 161  
910 | 7 (0.0%) | 0 (0%) | 7  
913 | 25 (0.0%) | 0 (0%) | 25  
915 | 2 (0.0%) | 0 (0%) | 2  
917 | 1 (0.0%) | 0 (0%) | 1  
920 | 7 (0.0%) | 0 (0%) | 7  
921 | 3 (0.0%) | 0 (0%) | 3  
922 | 3 (0.0%) | 0 (0%) | 3  
923 | 10 (0.0%) | 0 (0%) | 10  
925 | 117 (0.1%) | 0 (0%) | 117  
926 | 126 (0.1%) | 0 (0%) | 126  
927 | 1 (0.0%) | 0 (0%) | 1  
935 | 3 (0.0%) | 0 (0%) | 3  
936 | 11 (0.0%) | 0 (0%) | 11  
938 | 491 (0.3%) | 0 (0%) | 491  
940 | 31 (0.0%) | 0 (0%) | 31  
944 | 2 (0.0%) | 0 (0%) | 2  
945 | 2 (0.0%) | 0 (0%) | 2  
948 | 1,095 (0.7%) | 0 (0%) | 1,095  
949 | 736,873 (452.1%) | 0 (0%) | 736,873  
950 | 4 (0.0%) | 0 (0%) | 4  
951 | 1 (0.0%) | 0 (0%) | 1  
952 | 117 (0.1%) | 0 (0%) | 117  
954 | 1 (0.0%) | 0 (0%) | 1  
955 | 142 (0.1%) | 0 (0%) | 142  
963 | 9 (0.0%) | 0 (0%) | 9  
969 | 1,786 (1.1%) | 0 (0%) | 1,786  
978 | 1 (0.0%) | 0 (0%) | 1  
982 | 7 (0.0%) | 0 (0%) | 7  
985 | 11 (0.0%) | 0 (0%) | 11  
987 | 9 (0.0%) | 0 (0%) | 9  
989 | 1 (0.0%) | 0 (0%) | 1  
990 | 3 (0.0%) | 0 (0%) | 3  
991 | 19 (0.0%) | 0 (0%) | 19  
992 | 2 (0.0%) | 0 (0%) | 2  
994 | 1,187 (0.7%) | 0 (0%) | 1,187  
999 | 1,180,531 (724.3%) | 0 (0%) | 1,180,531  
</details>   
