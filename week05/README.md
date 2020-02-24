# Week 5

## Agenda
0. [Announcements](#announcements)
1. [Talking about homework/readings](#readings)
2. [Talking about the project](#project)
3. [QGIS Practice](#qgis) (This is ambitious.)
    * [Sharing Maps Outside of QGIS](#qgis1)
    * [Drawing your own polygons](#qgis2)
    * [Fixing Broken Shapefiles](#qgis3)
4. [Homework/Readings](#homework)
 
## <span id="announcements">Announcements</span>

On March 5th at 4pm, the DAT faculty are convening to start the process of rebuilding our curriculum. Some things will stay the same (e.g. I don't imagine DAT-102 will be entirely reimagined from scratch, but some of the higher-level courses will need major facelifts). Students are invited to show up then; for those folks who aren't available then, you're also welcome to give us comments that we should take into account when we're doing the redesign. 

## <span id="readings">Talking about homework</span>

Did everyone get through the exercise looking at the digital divide in PA? Who is willing to share your map with the class? What does the data tell you?  

I gave you two weeks for the readings, and I'll repeat them below, so we won't discuss them yet unless you've got questions.

## <span id="project">Talking about the project</span>

As promised, [here is the specification of the project](../files/map_mini_project_specification.md).

Let's go around the room to find out who has a topic that interests them, and let's see if we can get groups together using just that information. 

## <span id="qgis">QGIS Practice</span>
    
Note: we're doing all of this (at least, all that we are able) in class, together. I wrote it out in case that's easier for you, or you want to remind yourself how to do some of this later.

You're going to want to open GitHub on the browser _on the machine where you're running QGIS_. (Are you running it on the VM? Open it in Firefox on the VM.)

    
### <span id="qgis1">Sharing Maps Outside of QGIS</span>

We will want to communicate with people who don't have QGIS, sometimes. Creating print map layouts will help us do so effectively.

For this exercise you can choose any of the maps you've created in class or for homework. I will use the map showing percentage of households without internet that we created last session, but you are not constrained by my choices, here.

1. Open the project you want to create a map of.
1. Zoom in/out until the area you want to map is taking up most of the map panel.
1. Go to Project -> New Print Layout, and give your print layout a title. This title will be the default filename for your map when you export it to PDF (or JPG, but use PDF). It will also be how you pull it back up when you want to re-export.
1. To add your map to your layout, go to Add Item -> Add Map.
    * When you mouse over the page on the screen, crosshairs will appear.
    * Hold down the left mouse button and drag to select how much of your page your map will take up. You'll be able to resize and reposition as needed, later.
    * If you don't like the extent of your map, you can fiddle with it under the Item Properties tab, in the "Extents" section. 
1. When you have your map on your page, go ahead and save.
1. Now let's add a legend using the Add Item menu.
    * Consider changing its title to something more helpful (or at least "Legend") under Item Properties -> Title. If you use a long title, you can add a character to wrap on. (On one map I wrapped on the character "x" and used the title "Households xWithout Internet")
    * Under Legend Items, you have the option to turn layers/groups on and off by right-clicking and choosing "Hidden." (QGIS will probably require you to turn off "Auto Update" first.)
    * You can also relabel your layers by clicking the pencil-and-paper button below the Legend Items box.
1. If you'd like to add a compass rose, you can go to Add Item -> Add Picture, and the ellipsis to choose a file should take you to a pre-loaded list of pictures. (If your QGIS, like my QGIS, fails to do this by default, and if you're on Windows, you can find them in C:\Program Files\QGIS [number]\apps\qgis\svg. The path on the Linux machines is /usr/share/qgis/svg/, and I'll show you in class how I figured that out.) You can try several out, to see which you like.
1. A title, other commentary, citations for data sources, and any other text labels you might like to add are under Add Item -> Add Label. You can use HTML markup to style your text--remember to check the "Render as HTML" box.
1. Once you've added items to your heart's content and you're ready to make a sharable map, go to Layout -> Export as PDF.

If you want to make an overview map, the directions are very similar; only, you'll add your zoomed-in area as a map, and then you'll zoom back out and add a second map. Do yourself a favor, and lock your first map before you do this.

1. With the second (overview/large area) map selected, in the Item Properties tab, open the Overviews dropdown.
1. Click the plus mark to add an overview. (You can double-click and name it something more descriptive than "Overview 1," if you choose to do so.)
1. Assuming the wide area map is Map 2 and the zoomed-in area map is Map 1, you'll choose Map 1 as your Map frame.
1. Choose a Frame Style that makes sense. (Simple fill in red is often a default, but if you're doing this on a map that's colored in shades of red, you might choose a different color/style.)
1. Blending Mode might look familiar if you've used Photoshop in the past. Try a few different ones and see what looks best. I seem to be mostly drawn to Normal and Burn.


### <span id="qgis2">Drawing your own polygons</span>

We're going to draw a couple of Canadian provinces (because they're easier than most states, and we can all use a brush up on Canadian geography).

1. Start a new project.
1. Add OpenStreetMap (under XYZ Tiles) as a layer.
1. Create a new shapefile layer. (Layer -> Create Layer -> New Shapefile Layer)
    * Save it as "provinces.shp" in the directory you're working in tonight.
    * Set it as a polygon geometry type.
    * Add fields "id" (whole number) and "name" (text).
    * Note: Canada is kind of far north. There is definitely a better projection to use, but for now, even though we know better, we'll stick with the project's CRS -- EPSG 3857, Pseudo-Mercator.
1. Make sure you have the Digitizing Toolbar and Snapping Toolbar turned on (View -> Toolbars, and make sure both are checked)
1. In the Digitizing Toolbar, enable editing (pencil) and choose the Add Polygon Feature tool (looks like a golf course or a green swimming pool with a little orange star under it)
1. Trace Saskatchewan. Left-click at one of the top corners, and click at each point where you want there to be a vertex. (Remember: a polygon is just a bunch of lines, and a line is defined by two points.) After you've made it to the final corner, right-click to tell the tool you're finished, and a little table will pop up, asking you to enter an id (1) and the name of the province.
1. Now, before we start Alberta, do yourself a favor, and turn on the Enable Snapping tool (looks like a horseshoe or magnet)
1. Now you can snap to the top left corner of Saskatchewan, to start drawing Alberta. It'll also snap to the bottom left corner when you finish.

### <span id="qgis3">Fixing Broken Shapefiles</span>

First, I verify and clean up the directions. Then I post them.

## <span id="homework">Homework and Readings</span>

### Practice with QGIS on your own:

Look through the [PASDA](http://www.pasda.psu.edu/) data sets, and make a map and a data-based assertion that's interesting to you. (If you want to use [WPRDC](https://data.wprdc.org/dataset) instead, you can.) If none of the data sets speak to you, please look at how many [oil and gas](http://www.pasda.psu.edu/uci/DataSummary.aspx?dataset=283) or [coal](http://www.pasda.psu.edu/uci/DataSummary.aspx?dataset=271) operations are being run in the [Chesapeake Bay watershed](http://www.pasda.psu.edu/uci/DataSummary.aspx?dataset=59) (or Allegheny County or any other subset of the state of interest to you). There are also [oil and gas water pollution control facilities](http://www.pasda.psu.edu/uci/DataSummary.aspx?dataset=284), if you'd like to look at those. Don't forget to cite your data sources, and keep a log of the changes you make, so that another data analyst could follow your steps. 

Try making an attractive layout of your PASDA-data-based map that tells the story you intend to tell. 

Put your map, log, and layout into a folder (please put your first name and NOT your last name somewhere in the name of the folder), and upload it to [our shared directory](https://acdccac-my.sharepoint.com/personal/edarsow_acd_ccac_edu/_layouts/15/onedrive.aspx?originalPath=aHR0cHM6Ly9hY2RjY2FjLW15LnNoYXJlcG9pbnQuY29tLzpmOi9nL3BlcnNvbmFsL2VkYXJzb3dfYWNkX2NjYWNfZWR1L0VrUzQzNF9LMVV4RnZjbDBQNEI5WjAwQnMwV2dkRjF1MDZpQTdKZFJxbEtXR2c%5FcnRpbWU9eko3alpIQ3gxMGc&viewid=e2ddbbdb%2D20ac%2D4c4b%2D9dff%2Db8735d690d4b&id=%2Fpersonal%2Fedarsow%5Facd%5Fccac%5Fedu%2FDocuments%2Fdata%5Fanalytics%2Fdat%5F201%5F20sp%5Fstudent%5Fwork), inside the folder "maps!" -> "practice_maps."

### Readings (OK, I did add one, but it's fun) - we'll discuss next week

* [What's in a map?](https://www.gislounge.com/whats-in-a-map/)
* [Design principles for cartography](https://www.esri.com/arcgis-blog/products/product/mapping/design-principles-for-cartography/)
* [The Incline - Pittsburgh Maps Edition](https://theincline.com/newsletter/2020-02-13-the-pittsburgh-maps-edition/)