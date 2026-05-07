---
title: C. Import this data into Gephi
parent: Visualizing a Network Dataset Using Gephi
layout: default
nav_order: 3
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2021-09-13
---

C. Import this data into Gephi
------------------------------

1. First, let’s start up Gephi (we can search for it in the Windows Programs menu if we don’t see a desktop shortcut).
2. We should see a welcome screen where we can revisit recent projects or look at sample datasets.

    <img src='{{ '/assets/images/Gephi_C_002.1.png' | relative_url }}' alt="The Gephi application with the 'Welcome' startup menu." title='' width='600' height='369' />

    We can also use this screen to open up a graph file, if we had one. In our case, we want to create a new project, so click on **New Project** from this screen.

    <img src='{{ '/assets/images/Gephi_C_002.2.png' | relative_url }}' alt="Gephi's welcome startup window with the 'New Project' link highlighted." title='' width='600' height='335' />

    If we had closed this window by mistake, we can also use **File->New Project**.

    <img src='{{ '/assets/images/Gephi_C_002.3.png' | relative_url }}' alt="Gephi's top menu with 'New Project', listed underneath 'File', highlighted." title='' width='400' height='353' />
3. Along the top, we notice there are three tabs – Overview, Data Laboratory, and Preview. Let’s look at the **Data Laboratory** tab first to load some data.

    <img src='{{ '/assets/images/Gephi_C_003.1.png' | relative_url }}' alt="The 'Data Laboratory' button underneath Gephi's top menu highlighted." title='' width='600' height='198' />

    We are going to load the nodes and edges data we have for Romeo and Juliet. Click on the **Import Spreadsheet** button at the top.

    <img src='{{ '/assets/images/Gephi_C_003.2.png' | relative_url }}' alt="The 'Import Spreadsheet' button near the top of the page, highlighted." title='' width='600' height='90' />

    Browse to the downloaded workshop files, into the **RomeoAndJuliet** folder, open up the **nodes.csv**, and then click on **Open**.

    <img src='{{ '/assets/images/Gephi_C_003.3.png' | relative_url }}' alt="The Open window with the 'nodes.csv' file selected. The 'Open' button near the bottom is highlighted." title='' width='600' height='374' />
4. Gephi opens up a wizard to help us load the data. It will show us a preview of the data. We can see that it says it is importing it as a Nodes table.

    <img src='{{ '/assets/images/Gephi_C_004.1.png' | relative_url }}' alt="Gephi's Wizard window with the 'Import as' and 'Preview' sections of the window highlighted. Underneath the 'Import as' section, the option 'Nodes table' has been selected." title='' width='600' height='385' />

    We are happy with these settings so click on **Next**.

    <img src='{{ '/assets/images/Gephi_C_004.2.png' | relative_url }}' alt="Gephi's Wizard window with the 'Next' button highlighted." title='' width='600' height='385' />
5. We will see a list of imported columns, and this is where we could change what columns are imported and their type, if it is incorrect. We want **Alliance** to be a string, so it is fine the way it is – no changes necessary. So click on **Finish**.

    <img src='{{ '/assets/images/Gephi_C_005.1.png' | relative_url }}' alt="Gephi's Wizard window with the 'Finish' button highlighted." title='' width='600' height='385' />
6. Finally, we will see a pop-up window that tells us if there were any issues with the import. This screen tells us how many nodes are in our graph = 19, which is helpful.  
  
    <img src='{{ '/assets/images/Gephi_C_006.1.png' | relative_url }}' alt="The Import Report window with the '# of Nodes' entry highlighted." title='' width='600' height='422' />

    We should select that we want to **Append** **to existing workspace**, instead of creating a new workspace, as we already have a new project and workspace open, and then click on **OK**.

    <img src='{{ '/assets/images/Gephi_C_006.2.png' | relative_url }}' alt="The Import Report window with the 'Append to existing workspace' option selected. The 'OK' button at the bottom of the window is highlighted." title='' width='600' height='421' />

    Now we should be able to see a preview of the nodes spreadsheet loaded.

    <img src='{{ '/assets/images/Gephi_C_006.3.png' | relative_url }}' alt='The resulting Data table with the imported nodes loaded.' title='' width='600' height='328' />
7. Next, we need to load the edges spreadsheet. Click on import spreadsheet, and select the **Edges.csv**. Again, Gephi will open up a wizard, showing a preview of the data and indicating that it is says it is importing it as an Edges table. Click on **Next**.  
  
    <img src='{{ '/assets/images/Gephi_C_007.1.png' | relative_url }}' alt="Gephi's Wizard window with the 'Import as' and 'Preview' sections of the window highlighted. Underneath the 'Import as' section, the option 'Edges table' has been selected." title='' width='600' height='385' />
8. Keep the defaults and click on **Finish**.  
  
    <img src='{{ '/assets/images/Gephi_C_008.1.png' | relative_url }}' alt="Gephi's Wizard window with the 'Finish' button highlighted." title='' width='600' height='385' />
9. Finally, we will see the window pop-up again to tell us if there are any issues. Here, we should specify that the **Graph Type** is Undirected for our edges (i.e., the relationship is mutual).  
  
    <img src='{{ '/assets/images/Gephi_C_009.1.png' | relative_url }}' alt="The popup window with the option 'Undirected' highlighted from the 'Graph Type' dropdown menu." title='' width='600' height='421' />

    We also see that we have 31 edges in our graph. Again, we want to select **Append to existing workspace**, and then click on **OK**. Upon clicking OK, a new window will show up stating that there were 0 mutual edges removed to fulfil the undirected type - disregard this by clicking **Close**. Now, the edges spreadsheet has been loaded.

    <img src='{{ '/assets/images/Gephi_C_009.2.png' | relative_url }}' alt="The popup window withe the '# of Edges' section, 'Append to existing workspace' section, and the 'OK' button highlighted." title='' width='600' height='421' />
10. We can toggle between the different tables using the Nodes and Edges buttons on the top left.  
  
    <img src='{{ '/assets/images/Gephi_C_010.1.png' | relative_url }}' alt="The top left 'Nodes' and 'Edges' buttons highlighted." title='' width='500' height='222' />

    If we toggle to show the edges table, we will see some extra columns have been added to specify the type of edge, in our case, undirected. There are also extra columns; for example, label, which we could have used for edge labels.

    <img src='{{ '/assets/images/Gephi_C_010.2.png' | relative_url }}' alt="The resulting data table with the 'Edges' button and 'Type' column name highlighted." title='' width='600' height='325' />

    Now our network data is loaded, and ready to visualize and analyze.

Technique: [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| Tools: [Gephi](https://mdlutoronto.github.io/tutorials-search/?tool=Gephi)