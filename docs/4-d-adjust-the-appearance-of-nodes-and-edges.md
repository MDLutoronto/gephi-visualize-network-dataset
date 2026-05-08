---
title: D. Adjust the appearance of nodes and edges
parent: Visualizing a Network Dataset Using Gephi
layout: default
nav_order: 4
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2021-09-13
---

D. Adjust the appearance of nodes and edges
-------------------------------------------

1. Next, let’s move to the **Overview** tab. This tab is where we do our network analysis, layout and visualizations.  
  
    <img src='{{ '/assets/images/Gephi_D_001.1.png' | relative_url }}' alt="The 'Overview' button underneath Gephi's top menu highlighted. The Gaphi graph pane now visible with nodes and edges." title='' width='600' height='368' />

    Let’s look at some of the tools along the edge of the graph pane, starting from the top left. The arrow icon is a direct selection tool and the rectangle allows you to draw a rectangle around the items you want selected. Once nodes are selected, then you can adjust their sizes and colours.

    <img src='{{ '/assets/images/Gephi_D_001.2.png' | relative_url }}' alt="The 'Direct Selection' tool located on the left of Graph pane, highlighted." title='' width='268' height='359' />
    <img src='{{ '/assets/images/Gephi_D_001.3.png' | relative_url }}' alt="The 'Rectangle Selection' tool located on the left of Graph pane, highlighted." title='' width='200' height='360' />
    

    For example, **use the rectangle tool** to draw a rectangle around all the nodes to select the whole graph.

    <img src='{{ '/assets/images/Gephi_D_001.4.png' | relative_url }}' alt='Rectangle selection box over the entire whole graph.' title='' width='600' height='528' />
2. Next, click on the icon that looks like a two sided arrow in a circle. This tool is called sizer and it can be used to adjust the sizes of nodes.  
  
    <img src='{{ '/assets/images/Gephi_D_002.1.png' | relative_url }}' alt="The 'Sizer' tool located on the left of Graph pane, highlighted." title='' width='200' height='398' />

    **Select the sizer tool.** Notice that the tool gives us a hint on how to operate it at the top of the pane.

    <img src='{{ '/assets/images/Gephi_D_002.2.png' | relative_url }}' alt='Tool hints at the top of the Gephi graph pane, highlighted.' title='' width='600' height='157' />

    **Click on the white space next to the graph and drag the mouse vertically**. All the nodes should be changing size.

    <img src='{{ '/assets/images/Gephi_D_002.3.png' | relative_url }}' alt='larger nodes on the Gephi graph pane.' title='' width='602' height='502' />
3. Another tool is a dragging hand icon. You can use it to move nodes around.  
  
    <img src='{{ '/assets/images/Gephi_D_003.1.png' | relative_url }}' alt="The 'Drag' tool located on the left of Graph pane, highlighted." title='' width='200' height='373' />

    Select it and then use this tool to **manually drag and reposition a node** in your graph.

    <img src='{{ '/assets/images/Gephi_D_003.2.png' | relative_url }}' alt='Node being moved with the drag tool on the Gephi graph pane.' title='' width='600' height='496' />
4. We can colour certain nodes manually by using the icon that looks like a paint brush – we can use this to highlight a specific node of interest.  
  
    <img src='{{ '/assets/images/Gephi_D_004.1.png' | relative_url }}' alt="The 'Painter' tool located on the left of Graph pane, highlighted." title='' width='200' height='359' />

    **Try selecting a node and colouring it red**. Every time you click on a node, it gets more vibrant.

    <img src='{{ '/assets/images/Gephi_D_004.2.png' | relative_url }}' alt="The Graph pane with one of the displayed graph's nodes red as opposed to its previous grey." title='' width='600' height='494' />
5. The next icon after the sizer icon is called brush. Note that when we hover over a tool, it describes how the tools works in a pop-up.  
  
    <img src='{{ '/assets/images/Gephi_D_005.1.png' | relative_url }}' alt="The 'Brush' tool located on the left of Graph pane, highlighted. The tool's description floats below it." title='' width='500' height='396' />

    In this case, it colours nodes and their nearest neighbour (i.e., directly connected) the same colour. Select the tool, change the colour at the top to blue, and then select a node.

    <img src='{{ '/assets/images/Gephi_D_005.2.png' | relative_url }}' alt="The 'Choose a Color' popup window, with a blue selected." title='' width='600' height='512' />

    Click multiple times as before to make the colour brighter.

    <img src='{{ '/assets/images/Gephi_D_005.3.png' | relative_url }}' alt="The Graph pane with three of the displayed graph's nodes with a blue hue." title='' width='600' height='495' />
6. The next two icons allow us to manually create a new node or a new edge. So, in theory we could draw out our network manually, instead of preparing node and edge spreadsheets. Unless your network is very small, this would be a labour-intensive process that could be prone to error.  
  
    <img src='{{ '/assets/images/Gephi_D_006.1.png' | relative_url }}' alt="The 'Node' and 'Edge' tools located on the left of Graph pane, highlighted." title='' width='200' height='357' />

7. We can reset colours on our graph using the grey rectangle icon near the bottom left of the graph pane. Click on that now.  
  
    <img src='{{ '/assets/images/Gephi_D_007.1.png' | relative_url }}' alt="The 'Reset colors' tool located on the bottom left of Graph pane, highlighted." title='' width='300' height='227' />
8. To colour nodes and edges in a graph based on specific attributes, use the appearance pane.  
  
    <img src='{{ '/assets/images/Gephi_D_008.1.png' | relative_url }}' alt="The 'Appearance' pane, located on the right of the 'Graph' pane, is highlighted." title='' width='500' height='453' />

    We can toggle between visualizing nodes and edges – let’s start with nodes. There are four ways you can affect the appearance of nodes: we can colour-code the nodes based on an attribute, such as alliance in our case, we can size the nodes based on an attribute, such as degree, and we can also affect the colour and size of labels on our nodes. Let's first take a look at colour. Select the painter’s palette icon. Here, the default is the Unique option, which will colour all the nodes a unique colour, in this case grey.

    <img src='{{ '/assets/images/Gephi_D_008.2.png' | relative_url }}' alt="The 'Color' button at the top of the 'Appearance' pane highlighted." title='' width='300' height='380' />

    Let’s try the Ranking option, where it will select a sequential colour palette (so one colour changing from light to dark) to show the range of a numeric variable. Select Ranking and choose **Degree** from the drop-down menu.

    <img src='{{ '/assets/images/Gephi_D_008.3.png' | relative_url }}' alt="In the 'Appearance' pane, the 'Ranking' option as well as 'Degree' option listed in the dropdown menu are both highlighted." title='' width='300' height='378' />

    Then click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_008.4.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='379' />

    You can see that the darker coloured nodes have more connections.

    <img src='{{ '/assets/images/Gephi_D_008.5.png' | relative_url }}' alt="The 'Apply' button at the bottom of the 'Appearance' pane is highlighted. The resulting colour-coded graph is also displayed." title='' width='600' height='496' />
9. However, colours are more effective when used for categorical data. For our example, we want to use partition and assign a qualitative colour palette where different colours match different categories. Let’s click on **Partition** and select the attribute **alliance**.  
  
    <img src='{{ '/assets/images/Gephi_D_009.1.png' | relative_url }}' alt="In the 'Appearance' pane, the 'Partition' option as well as 'alliance' option listed in the dropdown menu are both highlighted." title='' width='300' height='379' />

    We will see different colours assigned to correspond to different alliances. You can click on an individual colour to change it, or click on the palette link to select from predefined palettes. Let’s keep the default. Click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_009.2.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='378' />

    Now the nodes on your graph have been colour-coded correspond to different alliances.

    <img src='{{ '/assets/images/Gephi_D_009.3.png' | relative_url }}' alt="The 'Apply' button at the bottom of the 'Appearance' pane is highlighted. The resulting colour-coded graph is also displayed." title='' width='600' height='496' />
10. Using sizes in visualizations is an effective way of displaying numerical variables, so let’s size the nodes by a numeric attribute that we have: **Degree**. Click on the icon with multiple circles for node size.  
  
    <img src='{{ '/assets/images/Gephi_D_010.1.png' | relative_url }}' alt="The 'Size' button at the top of 'Appearance' pane, highlighted." title='' width='300' height='381' />

    The unique option is where you specify a set size for all nodes, but we want ranking where the node sizes will vary by degree. Click on **Ranking**, select **Degree** from the drop-down menu.

    <img src='{{ '/assets/images/Gephi_D_010.2.png' | relative_url }}' alt="In the 'Appearance' pane, the 'Ranking' option as well as 'Degree' option listed in the dropdown menu are both highlighted." title='' width='300' height='380' />

    Set the **Min size** to 20 and the **Max size** to 50, and then click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_010.3.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='313' />

    You can see that the nodes on your graph have been sized according to their different degrees.

    <img src='{{ '/assets/images/Gephi_D_010.4.png' | relative_url }}' alt="The minimum and maximum size and the 'Apply' button in the 'Appearance' pane are all highlighted. The resulting graph is also displayed." title='' width='600' height='500' />
11. So far we’ve been playing with node appearance. We could also adjust the edge appearance by selecting **Edges** in the appearance pane.  
  
    <img src='{{ '/assets/images/Gephi_D_011.1.png' | relative_url }}' alt="The 'Appearance' pane with the 'Edges' tab highlighted." title='' width='300' height='373' />

    There are several options to change colours and adjust labels. We could for example just colour all our edges grey by selecting **Unique** for colour and keeping the default grey colour specified and then clicking on **Apply**. However, we have an attribute for our edges, so for our graph let’s use partition to colour them by relationship type. Click on **Partition** for colour, and then select **relationship**.

    <img src='{{ '/assets/images/Gephi_D_011.2.png' | relative_url }}' alt="In the 'Appearance' pane, the 'Partition' option as well as 'relationship' option listed in the dropdown menu are both highlighted." title='' width='300' height='370' />

    Finally, click on **Apply**.

    <img src='{{ '/assets/images/Gephi_D_011.3.png' | relative_url }}' alt='In the Appearance panel, the Apply button highlighted. ' title='' width='300' height='371' />

    Now the edges on your graph have been colour-coded correspond to their different relationships.

    <img src='{{ '/assets/images/Gephi_D_011.4.png' | relative_url }}' alt="The 'Apply' button at the bottom of the 'Appearance' pane is highlighted. The resulting graph is also displayed." title='' width='600' height='501' />

Technique: [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| Tools: [Gephi](https://mdlutoronto.github.io/tutorials-search/?tool=Gephi)