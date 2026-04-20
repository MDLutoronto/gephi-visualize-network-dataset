---
title: E. Use layout algorithms
parent: Visualizing a Network Dataset Using Gephi
layout: default
nav_order: 5
---

E. Use layout algorithms
------------------------

1. When you first loaded the data, Gephi displayed the nodes and edges at random to start. You may find often that you need to adjust the layout of the nodes and edges of your graph so that you can start to make sense of the data visually and set the shape of your graph. Let's navigate to the layout pane.  
  
    <img src='{{ '/assets/images/Gephi_E_001.1.png' | relative_url }}' alt="The Gephi application with the 'Layout' pane at the bottom left highlighted." title='' width='600' height='369' />

    Select the drop down menu that says **Choose a layout**. Select an example, such as **Contraction**

    <img src='{{ '/assets/images/Gephi_E_001.2.png' | relative_url }}' alt="In the 'Layout' pane, the 'Contraction' entry is highlighted in the 'Choose a layout' dropdown menu." title='' width='300' height='475' />

    To get more information about the layout, hover over the blue circle with the “i”.

    <img src='{{ '/assets/images/Gephi_E_001.3.png' | relative_url }}' alt="The blue 'i' icon is highlighted with the 'Contraction' layout's description floating beside it." title='' width='300' height='473' />
2. From the layout list, we see two similarly named options: **Force Atlas** and **ForceAtlas 2**. Force-based algorithms follow a simple principle: linked nodes attract each other and non-linked nodes push apart. The Force Atlas layout is from Gephi – it works best for small networks (up to 10,000 nodes) and can be slow.  
  
    <img src='{{ '/assets/images/Gephi_E_002.1.png' | relative_url }}' alt="In the 'Layout' pane, the 'Force Atlas' entry is highlighted in the 'Choose a layout' dropdown menu." title='' width='300' height='483' />

    ForceAtlas 2 is an improved version that can handle larger networks, for up to a million nodes. For our graph, select **ForceAtlas 2**.

    <img src='{{ '/assets/images/Gephi_E_002.2.png' | relative_url }}' alt="In the 'Layout' pane, the 'Force Atlas 2' entry is highlighted in the 'Choose a layout' dropdown menu." title='' width='300' height='481' />

    *Note: Different algorithms are appropriate in different situations and for different types of data. Learn more about layouts* [*from Gephi’s website*](https://gephi.org/users/tutorial-layouts/)*.*
3. With any of these layout algorithms, there are settings we can play with to adjust how the algorithm works, such as settings that affect the attraction and repulsion of the nodes to each other and to the centre of the graph. The documentation will specify all the parameters – we can see short help snippets show up at the bottom of the pane when you click on a parameter.  
  
    <img src='{{ '/assets/images/Gephi_E_003.1.png' | relative_url }}' alt="In the 'Layout' pane, the 'Threads number' as well as the parameter's help snippet are both highlighted." title='' width='300' height='481' />

    Let’s select one of these parameters as an example, **Prevent Overlap**, so that none of our nodes overlap each other in the layout. Keep the rest of the defaults, and then click on **Run**.

    <img src='{{ '/assets/images/Gephi_E_003.2.png' | relative_url }}' alt="In the 'Layout' pane, the 'Prevent Overlap' option is selected. The 'Run' button, also in the pane, is highlighted." title='' width='300' height='481' />
4. We should see the graph change right before our eyes. The algorithm will continue to run and adjust the graph in small ways until we click on stop – so however long you run an algorithm can also have an effect on the layout. Let it run for 15 seconds or so, and then click on **Stop**.  
  
    <img src='{{ '/assets/images/Gephi_E_004.1.png' | relative_url }}' alt="The 'Stop' button in the 'Layout' pane is highlighted. The resulting graph is displayed in the Graph pane." title='' width='600' height='392' />
5. In our situation, our graph shrinks towards its centre. Click on the graph, and use the mouse wheel to quickly zoom in and out. If the graph is going off the edge of our screen, we can right click on the blank area and then drag to reposition our graph.  
  
    <img src='{{ '/assets/images/Gephi_E_005.1.png' | relative_url }}' alt="The 'dragging' tool being used within the Graph pane." title='' width='600' height='525' />

    We can click on the magnifying glass near the bottom left of the edge of the graph pane, to centre our graph on the screen – but watch out as it does sometimes zoom out again when you do that. Let’s zoom in and centre our graph.

    <img src='{{ '/assets/images/Gephi_E_005.2.png' | relative_url }}' alt="The 'Center on Graph' tool located on the bottom left of Graph pane, highlighted." title='' width='600' height='526' />