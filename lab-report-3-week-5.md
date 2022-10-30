# Lab report week 5! #
## Choose one from `less`, `find`, and `grep` ##
## **find** ##
* `-type`

*What it is doing?*

find in the directory the objects of particular type.

*Why it is useful?*

Quickily give us the output of a particular type.

**examples:**

1. input:

```
[cs15lfa22qe@ieng6-201]:technical:91$ find -type d
```

output:

```
.
./911report
./biomed
./government
./government/About_LSC
./government/Alcohol_Problems
./government/Env_Prot_Agen
./government/Gen_Account_Office
./government/Media
./government/Post_Rate_Comm
./plos
```

2. input:

```
[cs15lfa22qe@ieng6-201]:technical:100$ find -type f
```

output:

```
...

./government/Media/families_saved.txt
./government/Media/fight_domestic_abuse.txt
./government/Media/grants_fail_to_come.txt
./government/Media/help_rent-to-own_tenants.txt
./government/Media/highlight_Senior_Day.txt
./government/Media/less_legal_aid.txt
./government/Media/man_on_national_team.txt
./government/Media/not_accessible_to_disabled.txt
./government/Media/predatory_loans.txt
./government/Media/pro_bono_efforts.txt
./government/Media/residents_sue_city.txt
./government/Media/water_fees.txt
./government/Post_Rate_Comm/Cohenetal_Cost_Function.txt
./government/Post_Rate_Comm/Cohenetal_CreamSkimming.txt
./government/Post_Rate_Comm/Cohenetal_DeliveryCost.txt
./government/Post_Rate_Comm/Cohenetal_RuralDelivery.txt
./government/Post_Rate_Comm/Cohenetal_Scale.txt
./government/Post_Rate_Comm/Cohenetal_comparison.txt
./government/Post_Rate_Comm/Gleiman_EMASpeech.txt
./government/Post_Rate_Comm/Gleiman_gca2000.txt
./government/Post_Rate_Comm/Mitchell_6-17-Mit.txt
./government/Post_Rate_Comm/Mitchell_RMVancouver.txt
./government/Post_Rate_Comm/Mitchell_spyros-first-class.txt
./government/Post_Rate_Comm/Redacted_Study.txt
./government/Post_Rate_Comm/ReportToCongress2002WEB.txt
./government/Post_Rate_Comm/WolakSpeech_usps.txt
./plos/journal.pbio.0020001.txt
./plos/journal.pbio.0020010.txt
./plos/journal.pbio.0020012.txt
./plos/journal.pbio.0020013.txt
./plos/journal.pbio.0020019.txt
./plos/journal.pbio.0020028.txt
./plos/journal.pbio.0020035.txt
./plos/journal.pbio.0020040.txt
./plos/journal.pbio.0020042.txt
./plos/journal.pbio.0020043.txt
./plos/journal.pbio.0020046.txt
./plos/journal.pbio.0020047.txt
./plos/journal.pbio.0020052.txt
./plos/journal.pbio.0020053.txt
./plos/journal.pbio.0020054.txt
./plos/journal.pbio.0020063.txt
./plos/journal.pbio.0020064.txt
./plos/journal.pbio.0020067.txt
./plos/journal.pbio.0020068.txt
./plos/journal.pbio.0020071.txt
./plos/journal.pbio.0020073.txt
./plos/journal.pbio.0020100.txt
./plos/journal.pbio.0020101.txt
./plos/journal.pbio.0020105.txt
./plos/journal.pbio.0020112.txt
./plos/journal.pbio.0020113.txt
./plos/journal.pbio.0020116.txt
./plos/journal.pbio.0020121.txt
./plos/journal.pbio.0020125.txt
./plos/journal.pbio.0020127.txt
./plos/journal.pbio.0020133.txt
./plos/journal.pbio.0020140.txt
./plos/journal.pbio.0020145.txt
./plos/journal.pbio.0020146.txt
./plos/journal.pbio.0020147.txt
./plos/journal.pbio.0020148.txt
./plos/journal.pbio.0020150.txt
./plos/journal.pbio.0020156.txt
./plos/journal.pbio.0020161.txt
./plos/journal.pbio.0020164.txt
./plos/journal.pbio.0020169.txt
./plos/journal.pbio.0020172.txt
./plos/journal.pbio.0020183.txt
./plos/journal.pbio.0020187.txt
./plos/journal.pbio.0020190.txt
./plos/journal.pbio.0020206.txt
./plos/journal.pbio.0020213.txt
./plos/journal.pbio.0020214.txt
./plos/journal.pbio.0020215.txt
./plos/journal.pbio.0020216.txt
./plos/journal.pbio.0020223.txt
./plos/journal.pbio.0020224.txt
./plos/journal.pbio.0020228.txt
./plos/journal.pbio.0020232.txt
./plos/journal.pbio.0020241.txt
./plos/journal.pbio.0020262.txt
./plos/journal.pbio.0020263.txt
```

find all the files in the ./technical

3. `find -type (type) -name (name)`

input:

```
[cs15lfa22qe@ieng6-201]:technical:101$ find -type f -name "*73.txt"
```

output:

```
./biomed/bcr273.txt
./biomed/cc973.txt
./biomed/rr73.txt
./plos/journal.pbio.0020073.txt
./plos/pmed.0020073.txt
./plos/pmed.0020273.txt
```

find the files with name as desired.


* `-size`

*What it is doing?*

find the files which has size in some range

*Why it is useful?*

We can use it to select files with our desired size range. Particularly useful when the files' size differences are large.

**examples:**

1. input:

```
[cs15lfa22qe@ieng6-201]:technical:102$ find -size 10k
```

output:
```
./911report/preface.txt
./biomed/1472-6769-1-4.txt
./government/Gen_Account_Office/og96014.txt
./government/Gen_Account_Office/og96023.txt
./government/Gen_Account_Office/og96040.txt
./government/Gen_Account_Office/og96047.txt
./government/Gen_Account_Office/og97039.txt
./government/Gen_Account_Office/og97051.txt
./government/Gen_Account_Office/og97052.txt
./government/Media/Farm_workers.txt
./plos/journal.pbio.0020042.txt
./plos/journal.pbio.0020073.txt
./plos/journal.pbio.0020156.txt
./plos/journal.pbio.0020215.txt
./plos/journal.pbio.0020224.txt
./plos/journal.pbio.0020297.txt
./plos/journal.pbio.0030131.txt
./plos/pmed.0020005.txt
./plos/pmed.0020075.txt
```

Find files that are exactly 10 kb.

2. input:

```
[cs15lfa22qe@ieng6-201]:technical:108$ find -size -2k
```

output:
```
./plos/pmed.0020191.txt
./plos/pmed.0020226.txt
```

Find files that are less than 2 kb.

3. input:

```
[cs15lfa22qe@ieng6-201]:technical:110$ find -size +50k -size -53k
```

output:
```
./biomed/1471-2091-3-4.txt
./biomed/1471-2121-2-10.txt
./biomed/1471-2121-3-16.txt
./biomed/1471-2121-3-25.txt
./biomed/1471-2210-1-7.txt
./biomed/1476-069X-2-4.txt
./biomed/1476-072X-2-4.txt
./biomed/gb-2002-3-11-research0065.txt
./biomed/gb-2002-3-12-research0088.txt
./biomed/gb-2003-4-3-r17.txt
./government/Env_Prot_Agen/section-by-section_summary.txt
./government/Gen_Account_Office/June30-2000_gg00135r.txt
```

Find files in between 50 kb and 53 kb.


* `-iname`

*What it is doing?*

It searches for the files with name of desired regardless of case

*Why it is useful?*

We can use this to find the results we want when we are not sure what is in the directories. By using "-iname", we can prevent missing some suitable outputs.

**examples:**

1. input:

```
[cs15lfa22qe@ieng6-201]:technical:120$ find -iname *x*.txt
```

output:

```
./biomed/1471-213X-1-1.txt
./biomed/1471-213X-1-10.txt
./biomed/1471-213X-1-11.txt
./biomed/1471-213X-1-12.txt
./biomed/1471-213X-1-13.txt
./biomed/1471-213X-1-15.txt
./biomed/1471-213X-1-2.txt
./biomed/1471-213X-1-3.txt
./biomed/1471-213X-1-4.txt
./biomed/1471-213X-1-6.txt
./biomed/1471-213X-1-9.txt
./biomed/1471-213X-2-1.txt
./biomed/1471-213X-2-7.txt
./biomed/1471-213X-2-8.txt
./biomed/1471-213X-3-2.txt
./biomed/1471-213X-3-3.txt
./biomed/1471-213X-3-4.txt
./biomed/1471-213X-3-7.txt
./biomed/1471-230X-1-10.txt
./biomed/1471-230X-1-5.txt
./biomed/1471-230X-1-6.txt
./biomed/1471-230X-1-8.txt
./biomed/1471-230X-2-17.txt
./biomed/1471-230X-2-21.txt
./biomed/1471-230X-2-23.txt
./biomed/1471-230X-3-3.txt
./biomed/1471-230X-3-5.txt
./biomed/1471-244X-2-9.txt
./biomed/1471-244X-3-5.txt
./biomed/1472-684X-1-5.txt
./biomed/1472-684X-2-1.txt
./biomed/1472-684X-2-2.txt
./biomed/1475-925X-2-1.txt
./biomed/1475-925X-2-10.txt
./biomed/1475-925X-2-11.txt
./biomed/1475-925X-2-12.txt
./biomed/1475-925X-2-3.txt
./biomed/1475-925X-2-6.txt
./biomed/1476-069X-1-3.txt
./biomed/1476-069X-2-2.txt
./biomed/1476-069X-2-4.txt
./biomed/1476-069X-2-7.txt
./biomed/1476-069X-2-9.txt
./biomed/1476-072X-2-3.txt
./biomed/1476-072X-2-4.txt
./biomed/1476-511X-1-2.txt
./biomed/1476-511X-2-2.txt
./biomed/1476-511X-2-3.txt
./government/Env_Prot_Agen/atx1-6.txt
./government/Media/Barr_sharpening_ax.txt
./government/Media/Rumble_in_the_Bronx.txt
./government/Media/Texas_Lawyer.txt
./government/Media/Texas_Supreme_Court.txt
./government/Media/agency_expands.txt
```

Find all the files which contains x in their name regardless of case.

2. input:

```
[cs15lfa22qe@ieng6-201]:technical:122$ find -iname comm*.txt
```

output:
```
./government/About_LSC/Comments_on_semiannual.txt
./government/About_LSC/commission_report.txt
./government/Media/CommercialAppealMemphis2.txt
./government/Media/Commercial_Appeal.txt
```

Find all the files which starts with "comm" regardless of case.

3. input:

```
[cs15lfa22qe@ieng6-201]:technical:124$ find -iname *onf*.txt
```

output:

```
./government/About_LSC/CONFIG_STANDARDS.txt
./government/About_LSC/conference_highlights.txt
```

Find all the files which contains "onf" in their name regardless of case.

