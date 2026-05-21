---
title: F. Add labels and make final layout adjustments
parent: Visualizing a Network Dataset Using Gephi
layout: default
nav_order: 6
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2021-09-13
---

F. Add labels and make final layout adjustments
-----------------------------------------------

1. Now, let’s look at node labels and the icons on the bottom of the graph pane edge. Click on the black 'T' icon to show node labels.  
  
    <img src='{{ '/assets/images/Gephi_F_001.1.png' | relative_url }}' alt="The 'Show Nodes Labels' tool located on the bottom of Graph pane, highlighted." title='' width='600' height='527' />

    Gephi will take the text from the label column we created in our nodes spreadsheet.

    <img src='{{ '/assets/images/Gephi_F_001.2.png' | relative_url }}' alt="The 'Size mode' tool located on the bottom left of Graph pane, highlighted." title='' width='600' height='527' />

    Then click on the black 'A' icon and select **Node size** – so they will be proportional to the node sizes.

    <img src='{{ '/assets/images/Gephi_F_001.3.png' | relative_url }}' alt='The Node size option in the Size Mode drop down menu located on the bottom of the Graph pane, highlighted.' title='' width='600' height='233' />

    Then use the slider on the right of that icon to make the node labels smaller and more readable.

    <img src='{{ '/assets/images/Gephi_F_001.4.png' | relative_url }}' alt='The slider located on the bottom of the Graph pane, highlighted.' title='' width='600' height='525' />

    We can also change the font, its size, and colour from here.
2. Layouts can help us make your labels more legible. Go back to the Layout pane and run **Label Adjust**.  
  
    <img src='{{ '/assets/images/Gephi_F_002.1.png' | relative_url }}' alt="In the 'Layout' pane, the 'Label Adjust' entry is highlighted in the 'Choose a layout' dropdown menu." title='' width='300' height='475' />

    Then run **Noverlap**. Use the blue “i” icon to learn more about these and other layouts.

    <img src='{{ '/assets/images/Gephi_F_002.2.png' | relative_url }}' alt="The blue 'i' icon is highlighted with the 'Nonoverlap' layout's description floating beside it." title='' width='300' height='474' />

    After we run those layouts, we might need to zoom out a bit. At this point, we can also use the grabbing hand icon near the top left edge of the graph pane to make some final tweaks to the layout by moving individual nodes.

    <img src='{{ '/assets/images/Gephi_F_002.3.png' | relative_url }}' alt="The 'Dragging' tool located on the left of Graph pane, highlighted." title='' width='600' height='525' />
3. Let’s go back to the graph pane icons. The little clipboard next to the node label colour selector allows you to specify which attribute to display as a label – the default is the label column.  
  
    <img src='{{ '/assets/images/Gephi_F_003.1.png' | relative_url }}' alt="The 'Attributes' tool located at the bottom of Graph pane, highlighted." title='' width='600' height='115' />
4. The white T turns on edge labels, but we are not going to label our edges in this situation.  
  
    <img src='{{ '/assets/images/Gephi_F_004.1.png' | relative_url }}' alt="The 'Show Edge Labels' tool located at the bottom of Graph pane, highlighted." title='' width='600' height='115' />

    The sliders adjusts the thickness of our edges – we can make them a bit thicker to see the colours better.

    <img src='{{ '/assets/images/Gephi_F_004.2.png' | relative_url }}' alt="The 'Edge Weight Scale' located at the bottom of Graph pane, highlighted." title='' width='600' height='115' />

    We already coloured all our edges by their relationship type, but if we had wanted, we could have coloured our edges by the source node (which is more helpful in directed graphs), by selecting the rainbow icon.

    <img src='{{ '/assets/images/Gephi_F_004.3.png' | relative_url }}' alt="The 'Edges have source node color' tool located at the bottom of Graph pane, highlighted." title='' width='600' height='117' />

    The icon to the left allows us to toggle the edges off and on in our graph – helpful for working with and viewing very complicated graphs.

    <img src='{{ '/assets/images/Gephi_F_004.4.png' | relative_url }}' alt="The 'Show edges' tool located at the bottom of Graph pane, highlighted." title='' width='600' height='117' />
5. The lightbulb icon toggles the background between white and black.  
  
    <img src='{{ '/assets/images/Gephi_F_005.1.png' | relative_url }}' alt="The 'Background color' tool located at the bottom of Graph pane, highlighted." title='' width='600' height='117' />

    Click it to try it out. You can see the background of your graph has toggled to black, and the label text has toggled to white to keep it readable.

    <img src='{{ '/assets/images/Gephi_F_005.2.png' | relative_url }}' alt="The effects of the 'Background color' tool, the graph with a black background and white labels, is displayed." title='' width='600' height='525' />

    The blue 'A' icon allows us to link node label colours to node colours, but in this case let’s leave the default as the black labels are more legible.

    <img src='{{ '/assets/images/Gephi_F_005.3.png' | relative_url }}' alt="The 'Color mode' tool located at the bottom of Graph pane, highlighted." title='' width='600' height='117' />
6. If you click on the little arrow icon on the far right, we can reveal even more options to play with, such as the ability to change how edges and nodes are coloured when they are selected.  
  
    <img src='{{ '/assets/images/Gephi_F_006.1.png' | relative_url }}' alt='The dropdown arrow at the bottom of the Graph pane is highlighted with the resulting menu.' title='' width='600' height='223' />
7. Additionally, there are a few icons to reset colours (which we saw before), along with icons to reset label colours and visibility, all near the bottom left edge of the graph pane.  
  
    <img src='{{ '/assets/images/Gephi_F_007.1.png' | relative_url }}' alt='The Reset Colours options in at the side of the Gephi graph pane, highlighted.' title='' width='600' height='117' />
8. We can see that we can use Gephi to visualize our network data to display the characters in a network and their relationships. Sizes and colours can be adjusted to illustrate attributes and then use the network diagrams to spot any spatial patterns. For example, the largest nodes (if node is sized by degree) could show us key entities in the network that have many connections. We could also see if the largest nodes are always the same colour (if we have colour-coded our nodes by a particular attribute) to see if there’s a relationship between that attribute and degree. Some limited analysis can be done visually and and convey interesting characteristics through our network diagrams.

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Gephi](https://mdlutoronto.github.io/tutorials-search/?tool=Gephi)