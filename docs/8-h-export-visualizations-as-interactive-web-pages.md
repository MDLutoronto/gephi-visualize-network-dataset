---
title: H. Export visualizations as interactive web pages
parent: Visualizing a Network Dataset Using Gephi
layout: default
nav_order: 8
staff:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
maintainer:
    - name: Kelly Schultz
      link: https://library.utoronto.ca/staff/kelly-schultz
created_date: 2021-09-13
---

H. Export visualizations as interactive web pages
-------------------------------------------------

1. Gephi can also create an interactive HTML web page (that can be hosted on a web server) using the **SigmaExporter** Plugin. To do so, first ensure that the plugin has been installed and is active. From the top menu, select **Tools** and then select **Plugins**.

    <img src='{{ '/assets/images/Gephi_H_001.1.png' | relative_url }}' alt="The 'Tools' menu with 'Plugins' selected and highlighted." title='' width='300' height='136' />

    Click on the **Installed** tab and ensure that SigmaExporter is listed.

    <img src='{{ '/assets/images/Gephi_H_001.2.png' | relative_url }}' alt="The plugins window with the 'Installed' tab open and SigmaExporter highlighted." title='' width='600' height='370' />

    If you are missing the Plugin, you can download it here from [Gephi’s website](https://gephi.org/plugins/#/plugin/sigmaexporter). For further guidance on this step, refer to [section A](https://mdlutoronto.github.io/gephi-visualize-network-dataset/1-a-set-up-gephi/) of this tutorial.
2. In the same **Plugins** window, now make sure that SigmaExporter is also active. Click on the **Installed** tab and check that a green checkmark appears in the Active column for SigmaExporter. If it doesn’t, check the box next to SigmaExporter and click on the **Activate** button underneath the list of plugins. Then close the plugins window.

    <img src='{{ '/assets/images/Gephi_H_002.1.png' | relative_url }}' alt="The plugins window with the 'Installed' tab open and SigmaExporter selected. Activate button below the plugin list highlighted." title='' width='600' height='370' />
3. To create an interactive visualization, go to the **File** menu, select Export and select **Sigma.js template...**

    <img src='{{ '/assets/images/Gephi_H_003.1.png' | relative_url }}' alt="The 'File' menu with 'Export' and 'Sigma.js template...' highlighted." title='' width='300' height='316' />
4. Click on the Browse button at the top and navigate to where you want to save the website, in our case, the **RomeoAndJuliet** folder.

    <img src='{{ '/assets/images/Gephi_H_004.1a.png' | relative_url }}' alt="SigmaExport window with 'Browse...' highlighted and opened. Save window with the RomeoAndJuliet folder selected." title='' width='600' height='557' />
5. For the **Legend** you can specify what the nodes, edges, and colours represent. In our case, write “Character” for **Node**, “Relationship” for **Edge** and “Alliance” for **Colour**.

    <img src='{{ '/assets/images/Gephi_H_005.1a.png' | relative_url }}' alt="SigmaExport window with the legend fields: Node, Edge, and Color filled in and highlighted." title='' width='600' height='555' />
6. Fill in information for the **Author**, **Title**, **Short Description** and **Long Description** fields.

    <img src='{{ '/assets/images/Gephi_H_006.1a.png' | relative_url }}' alt="SigmaExport window with the Author, Title, Short Description, and Long Description fields filled in and highlighted." title='' width='600' height='555' />
7. Select **alliance** from the **Group Selector** menu so that we can select nodes by alliance.

    <img src='{{ '/assets/images/Gephi_H_007.1a.png' | relative_url }}' alt="SigmaExport window with the Group Sector drop-down menu open and 'alliance' highlighted." title='' width='600' height='554' />
8. Keep all the other defaults for now and click **OK**.

    <img src='{{ '/assets/images/Gephi_H_008.1a.png' | relative_url }}' alt="SigmaExport window with 'OK' highlighted." title='' width='600' height='555' />
9. Open **Windows File Explorer** and navigate to the folder you just saved to. Within it, open the newly created **network** folder that contains the interactive web page. You would put these files on a web server to share them online with others. See the section below called **Viewing Exported Webpage** if you want to view and interact with the finished product locally first.  
  
    *Note: You can make adjustments to the node sizes, edge thickness, and label sizes by editing the config.json file, and adjustments to the node and edge colours by editing the data.json file.*
10. The last thing to do is to save our project as a .gephi file. Go to **File** and select **Save**, give it a name and select Gephi Files (*.gephi) from the Files of type drop-down menu. It saves our layout, colours, sizes and labels. And we are done!

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

**Technique:** [Data Visualization](https://mdlutoronto.github.io/tutorials-search/?technique=Data+Visualization) \| **Tools:** [Gephi](https://mdlutoronto.github.io/tutorials-search/?tool=Gephi)