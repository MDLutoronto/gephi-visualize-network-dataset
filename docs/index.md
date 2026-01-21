---
title: "Visualizing a Network Dataset Using Gephi"
layout: "home"
description: ""
permalink: "/"  #! Remove this if not the homepage
---

# Visualizing a Network Dataset Using Gephi

This tutorial will teach you the basic features in Gephi that will allow you to visualize network data. This tutorial is part of a longer workshop, “An Introduction to Network Visualization and Analysis.” You can [download the workshop materials](https://maps.library.utoronto.ca/workshops/GephiOnline/WorkshopFiles.zip) ([alternate workshop materials download](https://maps.library.utoronto.ca/datapub/workshops/GephiWorkshopFiles.zip)) and [watch the recording (1:44:18\)](https://play.library.utoronto.ca/23aef5db74b792db735a4f2fb39f7d7f) to learn more about network theory and see video demonstrations of working with Gephi.

For this tutorial, we are going to use Gephi to visualize a Romeo and Juliet network dataset. This dataset describes the strongest relationship between major characters in the play. We will learn how to import data into the tool, explore various icons and tools in the graph window, adjust the appearance of nodes and edges, use layout algorithms, add labels, and export final visualizations in various formats.

In this demonstration, we are going to:

[A. Set up Gephi](#SetUpGephi)  
[B. Download the tutorial dataset](#DownloadtheTutorialDataset)  
[C. Import this data into Gephi](#ImportDataintoGephi)  
[D. Adjust the appearance of nodes and edges](#AdjustappearanceNodesandEdges)  
[E. Use layout algorithms](#Uselayoutalgorithms)  
[F. Add labels and make final layout adjustments](#Addlabelsmakefinaladjustments)  
[G. Export visualizations as static images](#Exportasstaticimage)  
[H. Export visualizations as interactive web pages](#ExportInteractive)

This tutorial was created using Gephi version 0\.10\.1\.

 

A. Set up Gephi
---------------

1. This tutorial utilizes the free software package, [Gephi](https://gephi.org/), as well as the Gephi plugin, [SigmaExporter](https://gephi.org/plugins/#/plugin/sigmaexporter). If you already have these set up, skip ahead to [section B](#DownloadtheTutorialDataset) of this tutorial.
2. You can install Gephi, by [downloading it](https://gephi.org/users/download/), and following the [installation instructions](https://gephi.org/users/install/).
3. Once Gephi is set up, navigate to the application's top menu, select **Tools** and then select **Plugins**.

    <img src='{{ '/assets/images/Gephi_A_003.1.png' | relative_url }}' alt='Gephi's top menu with 'Tools' selected. From this selection a dropdown menu with the entry 'Plugins' is also selected.' title='' width='600' height='319' />
4. In the Plugins window, first select the**Available Plugins**, and navigate to**SignmaExporter.**Check the Install box, and click **Install**.

    <img src='{{ '/assets/images/Gephi_A_004.1.png' | relative_url }}' alt='The Plugins window with the Available Plugins tab highlighted and opened. SignmaExporter selected and Install highlighted.' title='' width='600' height='370' />
5. In the Plugin Installer, click **Next**, **accept the terms**, and click **Install**. You will need to restart the program before you use the plugin. After choosing your desired restart time, click **Finish**.

    <img src='{{ '/assets/images/Gephi_A_005.1.png' | relative_url }}' alt='The Plugin Installer window with the 'Finish' button highlighted.' title='' width='600' height='541' />

 

B. Download the tutorial dataset
--------------------------------

1. Create a new folder on your computer to store the workshop files.
2. [Download a zip file](https://maps.library.utoronto.ca/workshops/GephiOnline/WorkshopFiles.zip) containing all the datasets you will need for the workshop to that new folder.
3. Extract the files into that new folder.  
  
*Note: Different computers have different setups. On a Mac, just double\-click on the file to extract its files. On a PC, you might first want to install a great little program called* [*7\-Zip*](https://www.7-zip.org/) *(if you don't already have it!). Then you should be able to right click on the zip file and select 7\-Zip, then Extract Here to extract its files.*

 

C. Import this data into Gephi
------------------------------

1. First, let’s start up Gephi (we can search for it in the Windows Programs menu if we don’t see a desktop shortcut).
2. We should see a welcome screen where we can revisit recent projects or look at sample datasets.

    <img src='{{ '/assets/images/Gephi_C_002.1.png' | relative_url }}' alt='The Gephi application with the 'Welcome' startup menu.' title='' width='600' height='369' />

    We can also use this screen to open up a graph file, if we had one. In our case, we want to create a new project, so click on **New Project** from this screen.

    <img src='{{ '/assets/images/Gephi_C_002.2.png' | relative_url }}' alt='Gephi's welcome startup window with the 'New Project' link highlighted.' title='' width='600' height='335' />

    If we had closed this window by mistake, we can also use **File\-\>New Project**.

    <img src='{{ '/assets/images/Gephi_C_002.3.png' | relative_url }}' alt='Gephi's top menu with 'New Project', listed underneath 'File', highlighted.' title='' width='400' height='353' />
3. Along the top, we notice there are three tabs – Overview, Data Laboratory, and Preview. Let’s look at the **Data Laboratory** tab first to load some data.

    <img src='{{ '/assets/images/Gephi_C_003.1.png' | relative_url }}' alt='The 'Data Laboratory' button underneath Gephi's top menu highlighted.' title='' width='600' height='198' />

    We are going to load the nodes and edges data we have for Romeo and Juliet. Click on the **Import Spreadsheet** button at the top.

    <img src='{{ '/assets/images/Gephi_C_003.2.png' | relative_url }}' alt='The 'Import Spreadsheet' button near the top of the page, highlighted.' title='' width='600' height='90' />

    Browse to the downloaded workshop files, into the **RomeoAndJuliet** folder, open up the **nodes.csv**, and then click on **Open**.

    <img src='{{ '/assets/images/Gephi_C_003.3.png' | relative_url }}' alt='The Open window with the 'nodes.csv' file selected. The 'Open' button near the bottom is highlighted.' title='' width='600' height='374' />
4. Gephi opens up a wizard to help us load the data. It will show us a preview of the data. We can see that it says it is importing it as a Nodes table.

    <img src='{{ '/assets/images/Gephi_C_004.1.png' | relative_url }}' alt='Gephi's Wizard window with the 'Import as' and 'Preview' sections of the window highlighted. Underneath the 'Import as' section, the option 'Nodes table' has been selected.' title='' width='600' height='385' />

    We are happy with these settings so click on **Next**.

    <img src='{{ '/assets/images/Gephi_C_004.2.png' | relative_url }}' alt='Gephi's Wizard window with the 'Next' button highlighted.' title='' width='600' height='385' />
5. We will see a list of imported columns, and this is where we could change what columns are imported and their type, if it is incorrect. We want **Alliance** to be a string, so it is fine the way it is – no changes necessary. So click on **Finish**.

    <img src='{{ '/assets/images/Gephi_C_005.1.png' | relative_url }}' alt='Gephi's Wizard window with the 'Finish' button highlighted.' title='' width='600' height='385' />
6. Finally, we will see a pop\-up window that tells us if there were any issues with the import. This screen tells us how many nodes are in our graph \= 19, which is helpful.  
  
<img src='{{ '/assets/images/Gephi_C_006.1.png' | relative_url }}' alt='The Import Report window with the '# of Nodes' entry highlighted.' title='' width='600' height='422' />

    We should select that we want to **Append** **to existing workspace**, instead of creating a new workspace, as we already have a new project and workspace open, and then click on **OK**.

    <img src='{{ '/assets/images/Gephi_C_006.2.png' | relative_url }}' alt='The Import Report window with the 'Append to existing workspace' option selected. The 'OK' button at the bottom of the window is highlighted.' title='' width='600' height='421' />

    Now we should be able to see a preview of the nodes spreadsheet loaded.

    <img src='{{ '/assets/images/Gephi_C_006.3.png' | relative_url }}' alt='The resulting Data table with the imported nodes loaded.' title='' width='600' height='328' />
7. Next, we need to load the edges spreadsheet. Click on import spreadsheet, and select the **Edges.csv**. Again, Gephi will open up a wizard, showing a preview of the data and indicating that it is says it is importing it as an Edges table. Click on **Next**.  
  
<img src='{{ '/assets/images/Gephi_C_007.1.png' | relative_url }}' alt='Gephi's Wizard window with the 'Import as' and 'Preview' sections of the window highlighted. Underneath the 'Import as' section, the option 'Edges table' has been selected.' title='' width='600' height='385' />
8. Keep the defaults and click on **Finish**.  
  
<img src='{{ '/assets/images/Gephi_C_008.1.png' | relative_url }}' alt='Gephi's Wizard window with the 'Finish' button highlighted.' title='' width='600' height='385' />
9. Finally, we will see the window pop\-up again to tell us if there are any issues. Here, we should specify that the **Graph Type** is Undirected for our edges (i.e., the relationship is mutual).  
  
<img src='{{ '/assets/images/Gephi_C_009.1.png' | relative_url }}' alt='The popup window with the option 'Undirected' highlighted from the 'Graph Type' dropdown menu.' title='' width='600' height='421' />

    We also see that we have 31 edges in our graph. Again, we want to select **Append to existing workspace**, and then click on **OK**. Upon clicking OK, a new window will show up stating that there were 0 mutual edges removed to fulfil the undirected type \- disregard this by clicking **Close**. Now, the edges spreadsheet has been loaded.

    <img src='{{ '/assets/images/Gephi_C_009.2.png' | relative_url }}' alt='The popup window withe the '# of Edges' section, 'Append to existing workspace' section, and the 'OK' button highlighted.' title='' width='600' height='421' />
10. We can toggle between the different tables using the Nodes and Edges buttons on the top left.  
  
<img src='{{ '/assets/images/Gephi_C_010.1.png' | relative_url }}' alt='The top left 'Nodes' and 'Edges' buttons highlighted.' title='' width='500' height='222' />

    If we toggle to show the edges table, we will see some extra columns have been added to specify the type of edge, in our case, undirected. There are also extra columns; for example, label, which we could have used for edge labels.

    <img src='{{ '/assets/images/Gephi_C_010.2.png' | relative_url }}' alt='The resulting data table with the 'Edges' button and 'Type' column name highlighted.' title='' width='600' height='325' />

    Now our network data is loaded, and ready to visualize and analyze.

 

D. Adjust the appearance of nodes and edges
-------------------------------------------

1. Next, let’s move to the **Overview** tab. This tab is where we do our network analysis, layout and visualizations.  
  
<img src='{{ '/assets/images/Gephi_D_001.1.png' | relative_url }}' alt='The 'Overview' button underneath Gephi's top menu highlighted. The Gaphi graph pane now visible with nodes and edges.' title='' width='600' height='368' />

    Let’s look at some of the tools along the edge of the graph pane, starting from the top left. The arrow icon is a direct selection tool and the rectangle allows you to draw a rectangle around the items you want selected. Once nodes are selected, then you can adjust their sizes and colours.

    <img src='{{ '/assets/images/Gephi_D_001.2.png' | relative_url }}' alt='The 'Direct Selection' tool located on the left of Graph pane, highlighted.' title='' width='268' height='359' /><img src='{{ '/assets/images/Gephi_D_001.3.png' | relative_url }}' alt='The 'Rectangle Selection' tool located on the left of Graph pane, highlighted.' title='' width='200' height='360' />

    For example, **use the rectangle tool** to draw a rectangle around all the nodes to select the whole graph.

    <img src='{{ '/assets/images/Gephi_D_001.4.png' | relative_url }}' alt='Rectangle selection box over the entire whole graph.' title='' width='600' height='528' />
2. Next, click on the icon that looks like a two sided arrow in a circle. This tool is called sizer and it can be used to adjust the sizes of nodes.  
  
<img src='{{ '/assets/images/Gephi_D_002.1.png' | relative_url }}' alt='The 'Sizer' tool located on the left of Graph pane, highlighted.' title='' width='200' height='398' />

 **Select the sizer tool.** Notice that the tool gives us a hint on how to operate it at the top of the pane.

    <img src='{{ '/assets/images/Gephi_D_002.2.png' | relative_url }}' alt='Tool hints at the top of the Gephi graph pane, highlighted.' title='' width='600' height='157' />

 **Click on the white space next to the graph and drag the mouse vertically**. All the nodes should be changing size.

    <img src='{{ '/assets/images/Gephi_D_002.3.png' | relative_url }}' alt='larger nodes on the Gephi graph pane.' title='' width='602' height='502' />
3. Another tool is a dragging hand icon. You can use it to move nodes around.  
  
<img src='{{ '/assets/images/Gephi_D_003.1.png' | relative_url }}' alt='The 'Drag' tool located on the left of Graph pane, highlighted.' title='' width='200' height='373' />

    Select it and then use this tool to **manually drag and reposition a node** in your graph.

    <img src='{{ '/assets/images/Gephi_D_003.2.png' | relative_url }}' alt='Node being moved with the drag tool on the Gephi graph pane.' title='' width='600' height='496' />
4. We can colour certain nodes manually by using the icon that looks like a paint brush – we can use this to highlight a specific node of interest.  
  
<img src='{{ '/assets/images/Gephi_D_004.1.png' | relative_url }}' alt='The 'Painter' tool located on the left of Graph pane, highlighted.' title='' width='200' height='359' />

 **Try selecting a node and colouring it red**. Every time you click on a node, it gets more vibrant.

    <img src='{{ '/assets/images/Gephi_D_004.2.png' | relative_url }}' alt='The Graph pane with one of the displayed graph's nodes red as opposed to its previous grey.' title='' width='600' height='494' />
5. The next icon after the sizer icon is called brush. Note that when we hover over a tool, it describes how the tools works in a pop\-up.  
  
<img src='{{ '/assets/images/Gephi_D_005.1.png' | relative_url }}' alt='The 'Brush' tool located on the left of Graph pane, highlighted. The tool's description floats below it.' title='' width='500' height='396' />

    In this case, it colours nodes and their nearest neighbour (i.e., directly connected) the same colour. Select the tool, change the colour at the top to blue, and then select a node.

    <img src='{{ '/assets/images/Gephi_D_005.2.png' | relative_url }}' alt='The 'Choose a Color' popup window, with a blue selected.' title='' width='600' height='512' />

    Click multiple times as before to make the colour brighter.

    <img src='{{ '/assets/images/Gephi_D_005.3.png' | relative_url }}' alt='The Graph pane with three of the displayed graph's nodes with a blue hue.' title='' width='600' height='495' />
6. The next two icons allow us to manually create a new node or a new edge. So, in theory we could draw out our network manually, instead of preparing node and edge spreadsheets. Unless your network is very small, this would be a labour\-intensive process that could be prone to error.  
  
<img src='{{ '/assets/images/Gephi_D_006.1.png' | relative_url }}' alt='The 'Node' and 'Edge' tools located on the left of Graph pane, highlighted.' title='' width='200' height='357' />
7. We can reset colours on our graph using the grey rectangle icon near the bottom left of the graph pane. Click on that now.  
  
<img src='{{ '/assets/images/Gephi_D_007.1.png' | relative_url }}' alt='The 'Reset colors' tool located on the bottom left of Graph pane, highlighted. ' title='' width='300' height='227' />
8. To colour nodes and edges in a graph based on specific attributes, use the appearance pane.  
  
<img src='{{ '/assets/images/Gephi_D_008.1.png' | relative_url }}' alt='The 'Appearance' pane, located on the right of the 'Graph' pane, is highlighted.' title='' width='500' height='453' />

    We can toggle between visualizing nodes and edges – let’s start with nodes. There are four ways you can affect the appearance of nodes: we can colour\-code the nodes based on an attribute, such as alliance in our case, we can size the nodes based on an attribute, such as degree, and we can also affect the colour and size of labels on our nodes. Let's first take a look at colour. Select the painter’s palette icon. Here, the default is the Unique option, which will colour all the nodes a unique colour, in this case grey.

    <img src='{{ '/assets/images/Gephi_D_008.2.png' | relative_url }}' alt='The 'Color' button at the top of the 'Appearance' pane highlighted.' title='' width='300' height='380' />

    Let’s try the Ranking option, where it will select a sequential colour palette (so one colour changing from light to dark) to show the range of a numeric variable. Select Ranking and choose **Degree** from the drop\-down menu.

    <img src='{{ '/assets/images/Gephi_D_008.3.png' | relative_url }}' alt='In the 'Appearance' pane, the 'Ranking' option as well as 'Degree' option listed in the dropdown menu are both highlighted.' title='' width='300' height='378' />

    Then click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_008.4.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='379' />

    You can see that the darker coloured nodes have more connections.

    <img src='{{ '/assets/images/Gephi_D_008.5.png' | relative_url }}' alt='The 'Apply' button at the bottom of the 'Appearance' pane is highlighted. The resulting colour-coded graph is also displayed.' title='' width='600' height='496' />
9. However, colours are more effective when used for categorical data. For our example, we want to use partition and assign a qualitative colour palette where different colours match different categories. Let’s click on **Partition** and select the attribute **alliance**.  
  
<img src='{{ '/assets/images/Gephi_D_009.1.png' | relative_url }}' alt='In the 'Appearance' pane, the 'Partition' option as well as 'alliance' option listed in the dropdown menu are both highlighted.' title='' width='300' height='379' />

    We will see different colours assigned to correspond to different alliances. You can click on an individual colour to change it, or click on the palette link to select from predefined palettes. Let’s keep the default. Click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_009.2.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='378' />

    Now the nodes on your graph have been colour\-coded correspond to different alliances.

    <img src='{{ '/assets/images/Gephi_D_009.3.png' | relative_url }}' alt='The 'Apply' button at the bottom of the 'Appearance' pane is highlighted. The resulting colour-coded graph is also displayed.' title='' width='600' height='496' />
10. Using sizes in visualizations is an effective way of displaying numerical variables, so let’s size the nodes by a numeric attribute that we have: **Degree**. Click on the icon with multiple circles for node size.  
  
<img src='{{ '/assets/images/Gephi_D_010.1.png' | relative_url }}' alt='The 'Size' button at the top of 'Appearance' pane, highlighted.' title='' width='300' height='381' />

    The unique option is where you specify a set size for all nodes, but we want ranking where the node sizes will vary by degree. Click on **Ranking**, select **Degree** from the drop\-down menu.

    <img src='{{ '/assets/images/Gephi_D_010.2.png' | relative_url }}' alt='In the 'Appearance' pane, the 'Ranking' option as well as 'Degree' option listed in the dropdown menu are both highlighted.' title='' width='300' height='380' />

    Set the **Min size** to 20 and the **Max size** to 50, and then click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_010.3.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='313' />

    You can see that the nodes on your graph have been sized according to their different degrees.

    <img src='{{ '/assets/images/Gephi_D_010.4.png' | relative_url }}' alt='The minimum and maximum size and the 'Apply' button in the 'Appearance' pane are all highlighted. The resulting graph is also displayed.' title='' width='600' height='500' />
11. So far we’ve been playing with node appearance. We could also adjust the edge appearance by selecting **Edges** in the appearance pane.  
  
<img src='{{ '/assets/images/Gephi_D_011.1.png' | relative_url }}' alt='The 'Appearance' pane with the 'Edges' tab highlighted.' title='' width='300' height='373' />

    There are several options to change colours and adjust labels. We could for example just colour all our edges grey by selecting **Unique** for colour and keeping the default grey colour specified and then clicking on **Apply**. However, we have an attribute for our edges, so for our graph let’s use partition to colour them by relationship type. Click on **Partition** for colour, and then select **relationship**.

    <img src='{{ '/assets/images/Gephi_D_011.2.png' | relative_url }}' alt='In the 'Appearance' pane, the 'Partition' option as well as 'relationship' option listed in the dropdown menu are both highlighted.' title='' width='300' height='370' />

    Finally, click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_011.3.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='371' />

    Now the edges on your graph have been colour\-coded correspond to their different relationships.

    <img src='{{ '/assets/images/Gephi_D_011.4.png' | relative_url }}' alt='The 'Apply' button at the bottom of the 'Appearance' pane is highlighted. The resulting graph is also displayed.' title='' width='600' height='501' />

 

E. Use layout algorithms
------------------------

1. When you first loaded the data, Gephi displayed the nodes and edges at random to start. You may find often that you need to adjust the layout of the nodes and edges of your graph so that you can start to make sense of the data visually and set the shape of your graph. Let's navigate to the layout pane.  
  
<img src='{{ '/assets/images/Gephi_E_001.1.png' | relative_url }}' alt='The Gephi application with the 'Layout' pane at the bottom left highlighted.' title='' width='600' height='369' />

    Select the drop down menu that says **Choose a layout**. Select an example, such as **Contraction**

    <img src='{{ '/assets/images/Gephi_E_001.2.png' | relative_url }}' alt='In the 'Layout' pane, the 'Contraction' entry is highlighted in the 'Choose a layout' dropdown menu.' title='' width='300' height='475' />

    To get more information about the layout, hover over the blue circle with the “i”.

    <img src='{{ '/assets/images/Gephi_E_001.3.png' | relative_url }}' alt='The blue 'i' icon is highlighted with the 'Contraction' layout's description floating beside it.' title='' width='300' height='473' />
2. From the layout list, we see two similarly named options: **Force Atlas** and **ForceAtlas 2**. Force\-based algorithms follow a simple principle: linked nodes attract each other and non\-linked nodes push apart. The Force Atlas layout is from Gephi – it works best for small networks (up to 10,000 nodes) and can be slow.  
  
<img src='{{ '/assets/images/Gephi_E_002.1.png' | relative_url }}' alt='In the 'Layout' pane, the 'Force Atlas' entry is highlighted in the 'Choose a layout' dropdown menu.' title='' width='300' height='483' />

    ForceAtlas 2 is an improved version that can handle larger networks, for up to a million nodes. For our graph, select **ForceAtlas 2**.

    <img src='{{ '/assets/images/Gephi_E_002.2.png' | relative_url }}' alt='In the 'Layout' pane, the 'Force Atlas 2' entry is highlighted in the 'Choose a layout' dropdown menu.' title='' width='300' height='481' />

    *Note: Different algorithms are appropriate in different situations and for different types of data. Learn more about layouts* [*from Gephi’s website*](https://gephi.org/users/tutorial-layouts/)*.*
3. With any of these layout algorithms, there are settings we can play with to adjust how the algorithm works, such as settings that affect the attraction and repulsion of the nodes to each other and to the centre of the graph. The documentation will specify all the parameters – we can see short help snippets show up at the bottom of the pane when you click on a parameter.  
  
<img src='{{ '/assets/images/Gephi_E_003.1.png' | relative_url }}' alt='In the 'Layout' pane, the 'Threads number' as well as the parameter's help snippet are both highlighted.' title='' width='300' height='481' />

    Let’s select one of these parameters as an example, **Prevent Overlap**, so that none of our nodes overlap each other in the layout. Keep the rest of the defaults, and then click on **Run**.

    <img src='{{ '/assets/images/Gephi_E_003.2.png' | relative_url }}' alt='In the 'Layout' pane, the 'Prevent Overlap' option is selected. The 'Run' button, also in the pane, is highlighted.' title='' width='300' height='481' />
4. We should see the graph change right before our eyes. The algorithm will continue to run and adjust the graph in small ways until we click on stop – so however long you run an algorithm can also have an effect on the layout. Let it run for 15 seconds or so, and then click on **Stop**.  
  
<img src='{{ '/assets/images/Gephi_E_004.1.png' | relative_url }}' alt='The 'Stop' button in the 'Layout' pane is highlighted. The resulting graph is displayed in the Graph pane.' title='' width='600' height='392' />
5. In our situation, our graph shrinks towards its centre. Click on the graph, and use the mouse wheel to quickly zoom in and out. If the graph is going off the edge of our screen, we can right click on the blank area and then drag to reposition our graph.  
  
<img src='{{ '/assets/images/Gephi_E_005.1.png' | relative_url }}' alt='The 'dragging' tool being used within the Graph pane.' title='' width='600' height='525' />

    We can click on the magnifying glass near the bottom left of the edge of the graph pane, to centre our graph on the screen – but watch out as it does sometimes zoom out again when you do that. Let’s zoom in and centre our graph.

    <img src='{{ '/assets/images/Gephi_E_005.2.png' | relative_url }}' alt='The 'Center on Graph' tool located on the bottom left of Graph pane, highlighted.' title='' width='600' height='526' />

 

F. Add labels and make final layout adjustments
-----------------------------------------------

1. Now, let’s look at node labels and the icons on the bottom of the graph pane edge. Click on the black 'T' icon to show node labels.  
  
<img src='{{ '/assets/images/Gephi_F_001.1.png' | relative_url }}' alt='The 'Show Nodes Labels' tool located on the bottom of Graph pane, highlighted.' title='' width='600' height='527' />

    Gephi will take the text from the label column we created in our nodes spreadsheet.

    <img src='{{ '/assets/images/Gephi_F_001.2.png' | relative_url }}' alt='The 'Size mode' tool located on the bottom left of Graph pane, highlighted.' title='' width='600' height='527' />

    Then click on the black 'A' icon and select **Node size** – so they will be proportional to the node sizes.

    <img src='{{ '/assets/images/Gephi_F_001.3.png' | relative_url }}' alt='The Node size option in the Size Mode drop down menu located on the bottom of the Graph pane, highlighted.' title='' width='600' height='233' />

    Then use the slider on the right of that icon to make the node labels smaller and more readable.

    <img src='{{ '/assets/images/Gephi_F_001.4.png' | relative_url }}' alt='The slider located on the bottom of the Graph pane, highlighted.' title='' width='600' height='525' />

    We can also change the font, its size, and colour from here.
2. Layouts can help us make your labels more legible. Go back to the Layout pane and run **Label Adjust**.  
  
<img src='{{ '/assets/images/Gephi_F_002.1.png' | relative_url }}' alt='In the 'Layout' pane, the 'Label Adjust' entry is highlighted in the 'Choose a layout' dropdown menu.' title='' width='300' height='475' />

    Then run **Noverlap**. Use the blue “i” icon to learn more about these and other layouts.

    <img src='{{ '/assets/images/Gephi_F_002.2.png' | relative_url }}' alt='The blue 'i' icon is highlighted with the 'Nonoverlap' layout's description floating beside it.' title='' width='300' height='474' />

    After we run those layouts, we might need to zoom out a bit. At this point, we can also use the grabbing hand icon near the top left edge of the graph pane to make some final tweaks to the layout by moving individual nodes.

    <img src='{{ '/assets/images/Gephi_F_002.3.png' | relative_url }}' alt='The 'Dragging' tool located on the left of Graph pane, highlighted.' title='' width='600' height='525' />
3. Let’s go back to the graph pane icons. The little clipboard next to the node label colour selector allows you to specify which attribute to display as a label – the default is the label column.  
  
<img src='{{ '/assets/images/Gephi_F_003.1.png' | relative_url }}' alt='The 'Attributes' tool located at the bottom of Graph pane, highlighted.' title='' width='600' height='115' />
4. The white T turns on edge labels, but we are not going to label our edges in this situation.  
  
<img src='{{ '/assets/images/Gephi_F_004.1.png' | relative_url }}' alt='The 'Show Edge Labels' tool located at the bottom of Graph pane, highlighted.' title='' width='600' height='115' />

    The sliders adjusts the thickness of our edges – we can make them a bit thicker to see the colours better.

    <img src='{{ '/assets/images/Gephi_F_004.2.png' | relative_url }}' alt='The 'Edge Weight Scale' located at the bottom of Graph pane, highlighted.' title='' width='600' height='115' />

    We already coloured all our edges by their relationship type, but if we had wanted, we could have coloured our edges by the source node (which is more helpful in directed graphs), by selecting the rainbow icon.

    <img src='{{ '/assets/images/Gephi_F_004.3.png' | relative_url }}' alt='The 'Edges have source node color' tool located at the bottom of Graph pane, highlighted.' title='' width='600' height='117' />

    The icon to the left allows us to toggle the edges off and on in our graph – helpful for working with and viewing very complicated graphs.

    <img src='{{ '/assets/images/Gephi_F_004.4.png' | relative_url }}' alt='The 'Show edges' tool located at the bottom of Graph pane, highlighted.' title='' width='600' height='117' />
5. The lightbulb icon toggles the background between white and black.  
  
<img src='{{ '/assets/images/Gephi_F_005.1.png' | relative_url }}' alt='The 'Background color' tool located at the bottom of Graph pane, highlighted.' title='' width='600' height='117' />

    Click it to try it out. You can see the background of your graph has toggled to black, and the label text has toggled to white to keep it readable.

    <img src='{{ '/assets/images/Gephi_F_005.2.png' | relative_url }}' alt='The effects of the 'Background color' tool, the graph with a black background and white labels, is displayed.' title='' width='600' height='525' />

    The blue 'A' icon allows us to link node label colours to node colours, but in this case let’s leave the default as the black labels are more legible.

    <img src='{{ '/assets/images/Gephi_F_005.3.png' | relative_url }}' alt='The 'Color mode' tool located at the bottom of Graph pane, highlighted.' title='' width='600' height='117' />
6. If you click on the little arrow icon on the far right, we can reveal even more options to play with, such as the ability to change how edges and nodes are coloured when they are selected.  
  
<img src='{{ '/assets/images/Gephi_F_006.1.png' | relative_url }}' alt='The dropdown arrow at the bottom of the Graph pane is highlighted with the resulting menu.' title='' width='600' height='223' />
7. Additionally, there are a few icons to reset colours (which we saw before), along with icons to reset label colours and visibility, all near the bottom left edge of the graph pane.  
  
<img src='{{ '/assets/images/Gephi_F_007.1.png' | relative_url }}' alt='The Reset Colours options in at the side of the Gephi graph pane, highlighted.' title='' width='600' height='117' />
8. We can see that we can use Gephi to visualize our network data to display the characters in a network and their relationships. Sizes and colours can be adjusted to illustrate attributes and then use the network diagrams to spot any spatial patterns. For example, the largest nodes (if node is sized by degree) could show us key entities in the network that have many connections. We could also see if the largest nodes are always the same colour (if we have colour\-coded our nodes by a particular attribute) to see if there’s a relationship between that attribute and degree. Some limited analysis can be done visually and and convey interesting characteristics through our network diagrams.

 

G. Export visualizations as static images
-----------------------------------------

1. At this point, now that we have adjusted the appearance, we might want to export our visualization. The little camera icon at the bottom left of the main graph pane takes a snapshot of your graph as a PNG image file. Before clicking on it, select its drop\-down menu and click on **Configure**.  
  
<img src='{{ '/assets/images/Gephi_G_001.1.png' | relative_url }}' alt='Screenshot drop-down menu at the bottom of the Gephi graph pane open, with 'Configure' selected and highlighted.' title='' width='600' height='152' />

    If you keep the defaults and then use the snapshot tool, you will get a low\-resolution image; however, if instead you change the image size to 3000 by 2000 for example, and for the Antialiasing, try the maximum of 16x, the resulting snapshot will be a much higher resolution. Change those settings, click OK, and then click on the snapshot tool to take the image.

    <img src='{{ '/assets/images/Gephi_G_001.2.png' | relative_url }}' alt='Screenshot settings with 'Width' set to 3000, 'Height' set to 2000, and 'Antialiasing' set to 16x, all highlighted.' title='' width='300' height='320' />
2. If you want a higher quality image to export, you might need to use the **Preview** tab. Click on the **Preview** tab.

    <img src='{{ '/assets/images/Gephi_G_002.1.png' | relative_url }}' alt='The 'Preview' button underneath Gephi's top menu highlighted.' title='' width='600' height='242' />

    Depending on the plugins you have installed, Gephi may default to showing one of the plugins' panes as opposed to the "Preview Settings" pane. If Gephi defaults to another pane when you first click on the Preview tab, click on "Preview Settings".

    <img src='{{ '/assets/images/Gephi_G_002.2.png' | relative_url }}' alt='On the left pane, the 'Preview Settings' tab opened and highlighted.' title='' width='600' height='363' />
3. Click on the **Refresh** button at the bottom left to show the graph.  
  
<img src='{{ '/assets/images/Gephi_G_003.1.png' | relative_url }}' alt='Below the 'Preview Settings' pane, 'Refresh' highlighted. ' title='' width='600' height='567' />

    Here you might be surprised to notice that it does not look exactly like the graph you created in the Overview tab.

    <img src='{{ '/assets/images/Gephi_G_003.2.png' | relative_url }}' alt='The nodes and edges displayed in the 'Preview' pane.' title='' width='600' height='413' />

    You will have to use the options available on the left of this tab to prepare your visualization again for export.
4. First, we have lost our node labels. Under Node Labels on the left, select **Show Labels** and for the **Font**, select Arial, bold, size 3\.

    <img src='{{ '/assets/images/Gephi_G_004.1.png' | relative_url }}' alt='Under 'Node Labels' in 'Preview Settings', show labels selected and font settings opened, both highlighted. In font settings, 'Arial', 'Bold', and '3' selected and highlighted.' title='' width='600' height='472' />

    Click on the **Refresh** button again to see the changes.

    <img src='{{ '/assets/images/Gephi_G_004.2.png' | relative_url }}' alt='Below the 'Preview Settings' pane, 'Refresh' highlighted. ' title='' width='600' height='325' />
5. Next, let’s work on the edges, as they have lost their colours. Under Edges on the left, select **Color**, click on the ... button, select **Original** and then click on **OK**.

    <img src='{{ '/assets/images/Gephi_G_005.1.png' | relative_url }}' alt='Under 'Edge' in 'Preview Settings', Colour settings opened. Edge Color set to 'Original'.' title='' width='600' height='419' />

    Click on the **Refresh** button again to see the changes.

    <img src='{{ '/assets/images/Gephi_G_005.2.png' | relative_url }}' alt='Below the 'Preview Settings' pane, 'Refresh' highlighted. ' title='' width='600' height='325' />
6. As you can see there are many other options to try and experiment with to format the visualization.

    <img src='{{ '/assets/images/Gephi_G_006.1.png' | relative_url }}' alt='All the options in 'Preview Settings highlighted.' title='' width='300' height='728' />
7. When you are happy with it, click on SVG/PDF/PNG at the bottom next to Export. Let’s export it as a PDF file. Select your desired folder location and give the file a name.

    <img src='{{ '/assets/images/Gephi_G_007.1.png' | relative_url }}' alt='Below the 'Preview Settings' pane, 'Export' highlighted. In the Export window, save the save location, file name, and file type fields are all highlighted' title='' width='600' height='422' />

    Click on Options... Select Letter for the Page Size and make all the Margins 1 (to try to avoid labels being cut off at the edges, although you may need to play around with these settings, depending on your layout). Click on OK and then click on Save.

    <img src='{{ '/assets/images/Gephi_G_007.2.png' | relative_url }}' alt='In the export window, 'Options...' is opened and selected. In the 'Options PDF' window, page size is set to letter, and all margins are set to 1. ' title='' width='600' height='411' />
8. You should now have a PDF of your graph. When you open up the file, you will notice that there is no legend included. You would need to use a tool, such as [Adobe Illustrator](https://www.adobe.com/ca/products/illustrator.html) or [Inkscape](https://inkscape.org/) to add a legend to your graph.

 

H. Export visualizations as interactive web pages
-------------------------------------------------

1. Gephi can also create an interactive HTML web page (that can be hosted on a web server) using the **SigmaExporter** Plugin. To do so, first ensure that the plugin has been installed and is active. From the top menu, select **Tools** and then select **Plugins**.

    <img src='{{ '/assets/images/Gephi_H_001.1.png' | relative_url }}' alt='The 'Tools' menu with 'Plugins' selected and highlighted.' title='' width='300' height='136' />

    Click on the **Installed** tab and ensure that SigmaExporter is listed.

    <img src='{{ '/assets/images/Gephi_H_001.2.png' | relative_url }}' alt='The plugins window with the 'Installed' tab open and SigmaExporter highlighted.' title='' width='600' height='370' />

    If you are missing the Plugin, you can download it here from [Gephi’s website](https://gephi.org/plugins/#/plugin/sigmaexporter). For further guidance on this step, refer to [section A](#A) of this tutorial.
2. In the same **Plugins** window, now make sure that SigmaExporter is also active. Click on the **Installed** tab and check that a green checkmark appears in the Active column for SigmaExporter. If it doesn’t, check the box next to SigmaExporter and click on the **Activate** button underneath the list of plugins. Then close the plugins window.

    <img src='{{ '/assets/images/Gephi_H_002.1.png' | relative_url }}' alt='The plugins window with the 'Installed' tab open and SigmaExporter selected. Activate button below the plugin list highlighted.' title='' width='600' height='370' />
3. To create an interactive visualization, go to the **File** menu, select Export and select **Sigma.js template...**

    <img src='{{ '/assets/images/Gephi_H_003.1.png' | relative_url }}' alt='The 'File' menu with 'Export' and 'Sigma.js template...' highlighted.' title='' width='300' height='316' />
4. Click on the Browse button at the top and navigate to where you want to save the website, in our case, the **RomeoAndJuliet** folder.

    <img src='{{ '/assets/images/Gephi_H_004.1a.png' | relative_url }}' alt='SigmaExport window with 'Browse...' highlighted and opened. Save window with the RomeoAndJuliet folder selected.' title='' width='600' height='557' />
5. For the **Legend** you can specify what the nodes, edges, and colours represent. In our case, write “Character” for **Node**, “Relationship” for **Edge** and “Alliance” for **Colour**.

    <img src='{{ '/assets/images/Gephi_H_005.1a.png' | relative_url }}' alt='SigmaExport window with the legend fields: Node, Edge, and Color filled in and highlighted.' title='' width='600' height='555' />
6. Fill in information for the **Author**, **Title**, **Short Description** and **Long Description** fields.

    <img src='{{ '/assets/images/Gephi_H_006.1a.png' | relative_url }}' alt='SigmaExport window with the Author, Title, Short Description, and Long Description fields filled in and highlighted.' title='' width='600' height='555' />
7. Select **alliance** from the **Group Selector** menu so that we can select nodes by alliance.

    <img src='{{ '/assets/images/Gephi_H_007.1a.png' | relative_url }}' alt='SigmaExport window with the Group Sector drop-down menu open and 'alliance' highlighted.' title='' width='600' height='554' />
8. Keep all the other defaults for now and click **OK**.

    <img src='{{ '/assets/images/Gephi_H_008.1a.png' | relative_url }}' alt='SigmaExport window with 'OK' highlighted.' title='' width='600' height='555' />
9. Open **Windows File Explorer** and navigate to the folder you just saved to. Within it, open the newly created **network** folder that contains the interactive web page. You would put these files on a web server to share them online with others. See the section below called **Viewing Exported Webpage** if you want to view and interact with the finished product locally first.  
  
*Note: You can make adjustments to the node sizes, edge thickness, and label sizes by editing the config.json file, and adjustments to the node and edge colours by editing the data.json file.*
10. The last thing to do is to save our project as a .gephi file. Go to **File** and select **Save**, give it a name and select Gephi Files (\*.gephi) from the Files of type drop\-down menu. It saves our layout, colours, sizes and labels. And we are done!

**Viewing Exported Webpage Using Visual Studio Code** 
  
If you try to open up the newly exported index.html file to view it, you will find that it doesn’t display correctly. That is because newer web browsers block HTML files from running java script locally. There are a number of ways to get around this. Here is one option:

1. Install a free software package called [Visual Studio Code](https://code.visualstudio.com/)
2. Start it up
3. From the **Go** menu, select **Go to File**.
4. Type in the box: **ext install ritwickdey.liveserver**
5. Press Enter
6. Wait for the Live Server to install. It will indicate when it has finished installing on the left panel.
7. From the **File** menu, select **Open Folder…**
8. Browse to the network folder that you just exported and select it. Then click on the **Select Folder** button.
9. The contents of the folder should appear in the left panel. Right click on index.html and select **Open with Live Server**.
10. This should open up the file in your default browser, and you should be able to view it and interact with it.

Technique: [Data Visualization](/technique/data-visualization) \| Tools: [Gephi](/tools/gephi)**Date Created:** 2021\-09\-13**Updated:** 2024\-07\-17
