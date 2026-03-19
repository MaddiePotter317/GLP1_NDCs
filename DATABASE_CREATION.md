DATABASE CREATION


To create the NDC list for GLP1s I used the NIH website rxmix (https://mor.nlm.nih.gov/RxMix/) 


1. Create a text file with all of the GLP1 brand and generic names, with each name on one line. Save this file as GLP1_names. To get more information on how to gather the GLP1 names, see the GLP1 Details .md file. 

2. Open rxmix. On the site there is a section titled “Workflow”. Click the “function:” drop down menu and add findRXCUIbystring, this will have a pop up menu. In the allsrc box use 0- Active Concept, in the srclist box select all, and in search use 0- Exact Match Only, click add to workflow. Then add getRelatedByType this will have a pop up menu. In the tty box, select all, and in the expand box select nothing. Add this to workflow. Finally add GetAllHistoricalNDCs this will have a pop up menu. In the history box select 2 and click add to workflow. 

3. Then in the section labelled “Data”, select the “File” and upload your GLP1_name text file. Select Run and the NDCs and drug information will appear in the “Drug” section. Select the “download report” button and paste these results into a text file or excel file.  