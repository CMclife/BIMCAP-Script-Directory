# 263_VMT: FAMILY RENAMER

> #### DESCRIPTION: 
**Checks Naming Convention in Accordance to VMT BEP for: System & Inplace Families, Materials, Linestyle, Filled Regions, Links**

| File Category| Associated Files | Dynamo Packages | Author |
| :-------: | :----: | :---: | :---:
| 263_VMT | - | BumbleBee 2021.25.3| Cathrine Macabuhay |
|         | - | Clockwork 1.x 1.34.0|
|         | - | Crumple 2022.5.27   |
|         | - | Orchid 206.3.0.8161|
----------------------------------------------------------------
> #### SCRIPT: 

<details>
<summary>Script</summary>
<img src="/_images/vmt/VMTRenamer.png">
</details>

<details>
<summary>Inplace & System Families</summary>
<img src="/_images/vmt/VMTRFamilies.png">
</details>

<details>
<summary>Materials & Linestyle</summary>
<img src="/_images/vmt/VMTRMaterialsLineStyle.png">
</details>

<details>
<summary>Filled Regions & Fill Patterns</summary>
<img src="/_images/vmt/VMTRFilledRegionPatterns.png">
</details>

<details>
<summary>Links</summary>
<img src="/_images/vmt/VMTRLinks.png">
</details>

<details open>
<summary>Script Flow</summary>
<img src="/_images/vmt/VMTRStep.png">
</details>

> **System Family | Inplace Family | Materials | Filled Regions | Fill Pattern** 
- *01: Input: Excel Sheet from [**VMT : NamingConvention**:](/_vmt/VMTNamingConvention.md) 01.Incorrect Naming (Tab) & 02.Correct Naming (Tab)*
- *02: Get : Element ID & Correct Element Name*
- *03: Set : New Name*
- *04: Check : Double Check Naming Convention*
- *05: Output : Export to Excel (New Tab)*

<img src="/_images/vmt/VMTRLSStep.png">

> **LineStyles** 
- *01: Get : Line Styles in Project*
- *02: Replace : Multiple (Manual)*
- *03: Set : New Name*
- *04: Check : Double Check Naming Convention*
- *05: Output : Export to Excel (New Tab)*

<img src="/_images/vmt/VMTRLStep.png">

> **Links** 
- *01: Get : File Directory & Contents*
- *02: Get : File DirectoryName & FileName*
- *03: Set : New Name*
- *04: Check : Double Check Naming Convention*
- *05: Rename : Rename Files in Directory*
- *06: Output : Export to Excel (New Tab)*
------------------------------------------------------------------------------

> #### DEMO: 

> #### 01. SYSTEM FAMILY | INPLACE FAMILY | MATERIALS | FILL PATTERN | FILL REGIONS

<video width="1280" height="720" controls>
 <source src="/_demo/VMTR.mp4" type="video/mp4">
</video>

##### SCRIPT INSTRUCTIONS: 
- *01: Open Worksheet from previous Naming Convention Script - Duplicate "INCORRECT" Tab - Rename as "REVISED" and Rename all Incorrect Naming Conventions*
- *02: Open Dynamo Player : Select Script Folder Location*
- *02: Assign Excel Worksheet File Paths [Twice: 1)   "CORRECT" Naming 2) "INCORRECT" Naming Tabs]*
- *03: Run Script*
- *04: Script Automatically Renames Elements*
- *05: Script Will Export Secondary Naming Convention Checker into the Same Worksheet under a New Tab : "REVISED 02" for Anyother Naming Still Incorrect.*


> #### 02. LINESTYLE

<video width="1280" height="720" controls>
 <source src="/_demo/VMTRLS.mp4" type="video/mp4">
</video>

##### SCRIPT INSTRUCTIONS [LINESTYLE]: 
*- Need to Access Script Itself for Renaming -*
- *01: [Inside Script] Assign Naming Changes in the Codeblock - Connected to "LineStyle: String.ReplaceMultiple"*
- *02: Open Dynamo Player : Will Propmt you to Refresh*
- *03: Assign File Location of Previous Excel Sheet for LineStyle from Naming Convention*
- *03: Run Script*
- *04: Script Will Rename all [User Created] LineStyle Elements*
- *05: Script Will Export Secondary Naming Convention Checker into the Same Worksheet under a New Tab : "REVISED 02" for Anyother Naming Still Incorrect.*

> #### 03. LINKS

<video width="1280" height="720" controls>
 <source src="/_demo/VMTRL.mp4" type="video/mp4">
</video>

##### SCRIPT INSTRUCTIONS [LINKS]: 
*- Need to Access Script Itself for Renaming -*
- *01: [Inside Script] Assign Naming Changes in the Codeblock - Connected to "String.ReplaceMultiple"*
- *02: Open Dynamo Player : Will Propmt you to Refresh*
- *03: Input File Directory [Where the Links are located]*
- *03: Assign File Location of Previous Excel Sheet for Links from Naming Convention*
- *04: Script Will Rename all Links Existing in the Folder Directory*
- *05: Script Will Export Secondary Naming Convention Checker into the Same Worksheet under a New Tab : "REVISED 02" for Anyother Naming Still Incorrect.*