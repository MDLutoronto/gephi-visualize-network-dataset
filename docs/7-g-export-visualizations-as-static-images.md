---
title: G. Export visualizations as static images
parent: Visualizing a Network Dataset Using Gephi
layout: default
nav_order: 7
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2021-09-13
---

G. Export visualizations as static images
-----------------------------------------

1. At this point, now that we have adjusted the appearance, we might want to export our visualization. The little camera icon at the bottom left of the main graph pane takes a snapshot of your graph as a PNG image file. Before clicking on it, select its drop-down menu and click on **Configure**.  
  
    <img src='{{ '/assets/images/Gephi_G_001.1.png' | relative_url }}' alt="Screenshot drop-down menu at the bottom of the Gephi graph pane open, with 'Configure' selected and highlighted." title='' width='600' height='152' />

    If you keep the defaults and then use the snapshot tool, you will get a low-resolution image; however, if instead you change the image size to 3000 by 2000 for example, and for the Antialiasing, try the maximum of 16x, the resulting snapshot will be a much higher resolution. Change those settings, click OK, and then click on the snapshot tool to take the image.

    <img src='{{ '/assets/images/Gephi_G_001.2.png' | relative_url }}' alt="Screenshot settings with 'Width' set to 3000, 'Height' set to 2000, and 'Antialiasing' set to 16x, all highlighted." title='' width='300' height='320' />
2. If you want a higher quality image to export, you might need to use the **Preview** tab. Click on the **Preview** tab.

    <img src='{{ '/assets/images/Gephi_G_002.1.png' | relative_url }}' alt="The 'Preview' button underneath Gephi's top menu highlighted." title='' width='600' height='242' />

    Depending on the plugins you have installed, Gephi may default to showing one of the plugins' panes as opposed to the "Preview Settings" pane. If Gephi defaults to another pane when you first click on the Preview tab, click on "Preview Settings".

    <img src='{{ '/assets/images/Gephi_G_002.2.png' | relative_url }}' alt="On the left pane, the 'Preview Settings' tab opened and highlighted." title='' width='600' height='363' />
3. Click on the **Refresh** button at the bottom left to show the graph.  
  
    <img src='{{ '/assets/images/Gephi_G_003.1.png' | relative_url }}' alt="Below the 'Preview Settings' pane, 'Refresh' highlighted." title='' width='600' height='567' />

    Here you might be surprised to notice that it does not look exactly like the graph you created in the Overview tab.

    <img src='{{ '/assets/images/Gephi_G_003.2.png' | relative_url }}' alt="The nodes and edges displayed in the 'Preview' pane." title='' width='600' height='413' />

    You will have to use the options available on the left of this tab to prepare your visualization again for export.
4. First, we have lost our node labels. Under Node Labels on the left, select **Show Labels** and for the **Font**, select Arial, bold, size 3.

    <img src='{{ '/assets/images/Gephi_G_004.1.png' | relative_url }}' alt="Under 'Node Labels' in 'Preview Settings', show labels selected and font settings opened, both highlighted. In font settings, 'Arial', 'Bold', and '3' selected and highlighted." title='' width='600' height='472' />

    Click on the **Refresh** button again to see the changes.

    <img src='{{ '/assets/images/Gephi_G_004.2.png' | relative_url }}' alt="Below the 'Preview Settings' pane, 'Refresh' highlighted." title='' width='600' height='325' />
5. Next, let’s work on the edges, as they have lost their colours. Under Edges on the left, select **Color**, click on the ... button, select **Original** and then click on **OK**.

    <img src='{{ '/assets/images/Gephi_G_005.1.png' | relative_url }}' alt="Under 'Edge' in 'Preview Settings', Colour settings opened. Edge Color set to 'Original'." title='' width='600' height='419' />

    Click on the **Refresh** button again to see the changes.

    <img src='{{ '/assets/images/Gephi_G_005.2.png' | relative_url }}' alt="Below the 'Preview Settings' pane, 'Refresh' highlighted." title='' width='600' height='325' />
6. As you can see there are many other options to try and experiment with to format the visualization.

    <img src='{{ '/assets/images/Gephi_G_006.1.png' | relative_url }}' alt="All the options in 'Preview Settings highlighted." title='' width='300' height='728' />
7. When you are happy with it, click on SVG/PDF/PNG at the bottom next to Export. Let’s export it as a PDF file. Select your desired folder location and give the file a name.

    <img src='{{ '/assets/images/Gephi_G_007.1.png' | relative_url }}' alt="Below the 'Preview Settings' pane, 'Export' highlighted. In the Export window, save the save location, file name, and file type fields are all highlighted" title='' width='600' height='422' />

    Click on Options... Select Letter for the Page Size and make all the Margins 1 (to try to avoid labels being cut off at the edges, although you may need to play around with these settings, depending on your layout). Click on OK and then click on Save.

    <img src='{{ '/assets/images/Gephi_G_007.2.png' | relative_url }}' alt="In the export window, 'Options...' is opened and selected. In the 'Options PDF' window, page size is set to letter, and all margins are set to 1. " title='' width='600' height='411' />
8. You should now have a PDF of your graph. When you open up the file, you will notice that there is no legend included. You would need to use a tool, such as [Adobe Illustrator](https://www.adobe.com/ca/products/illustrator.html) or [Inkscape](https://inkscape.org/) to add a legend to your graph.

Technique: [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| Tools: [Gephi](https://mdlutoronto.github.io/tutorials-search/?tool=Gephi)