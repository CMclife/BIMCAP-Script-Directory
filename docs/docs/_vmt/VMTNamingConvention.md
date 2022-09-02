# 263_VMT: NAMING CONVENTION

> #### DESCRIPTION: 
**Checks Naming Convention in Accordance to VMT BEP for: System & Inplace Families, Materials, Linestyle, Filled Regions, Links and Exports Report into an Excel Worksheet.**

| File Category| Associated Files | Dynamo Packages | Author |
| :-------: | :----: | :---: | :---:
| 263_VMT | Excel Worksheet (for export) | BumbleBee 2021.25.3| Cathrine Macabuhay |
|         | - | Clockwork 1.x 1.34.0|
|         | - | Rhythm 2015.12.8   |
|         | - | Orchid 206.3.0.8161|
----------------------------------------------------------------
> #### SCRIPT: 

<details>
<summary>Script</summary>
<img src="/_images/vmt/VMTNamingConvention.png">
</details>

<details>
<summary>Inplace & System Families</summary>
<img src="/_images/vmt/VMTNCFamilies.png">
</details>

<details>
<summary>Materials & Linestyle</summary>
<img src="/_images/vmt/VMTNCMaterialsLineStyle.png">
</details>

<details>
<summary>Filled Regions & Fill Patterns</summary>
<img src="/_images/vmt/VMTNCFilledRegionPatterns.png">
</details>

<details>
<summary>Links</summary>
<img src="/_images/vmt/VMTNCLinks.png">
</details>

<details open>
<summary>Script Flow</summary>
<img src="/_images/vmt/VMTNCStep.png">
</details>

- *01: Retrieve Element*
- *02: Get : Category / Name / ID*
- *03: Check : Naming Convention*
- *04: Excel : Set Worksheet Header*
- *05: Output : Export Excel*
------------------------------------------------------------------------------

> #### DEMO: 

<video width="1280" height="720" controls>
 <source src="/_demo/VMTNC.mp4" type="video/mp4">
</video>

> #### NOTE : 
*All Naming Convention Reports are Exported to Excel Worksheets:*
- *01: Open Dynamo Player : Select Script Folder Location*
- *02: Assign Excel Worksheet File Paths*
- *03: Run Script*
- *04: Report Will Automatically Export onto Excel Worksheets*
- **Inplace Families Excel Will Automatically Open*