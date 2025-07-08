---
process_number: 180-03
title: CreatingClippedIndicatorMaps_20250508
author: Paulina Salinas Ruiz
created: 2025-05-08
modified: 2025-05-08
review_period: 3 years
---

**Purpose:**

This procedure outlines the process for creating indicator maps for the AERF Greening the Salish Sea Estuary Profiles in accordance with ISO 9000 quality management principles. The purpose of this procedure is to ensure efficiency in the creation and consistency in the display of the Estuary Profiles.

<table>
<colgroup>
<col style="width: 16%" />
<col style="width: 42%" />
<col style="width: 41%" />
</colgroup>
<thead>
<tr>
<th style="text-align: left;"><strong>Step</strong> </th>
<th style="text-align: left;"><strong>Major Activity</strong> </th>
<th style="text-align: left;"><strong>References, Forms and Details</strong> </th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;">1 </td>
<td>Save the original indicator map with another name (e.g. NRE_Indicator_Map en lieu de Indicator_Map) in ArcGIS Pro.</td>
<td></td>
</tr>
<tr>
<td style="text-align: center;">2 </td>
<td>Create extent with a polygon</td>
<td><ol type="a">
<li><p>Click on the Insert tab, choose Polygon Map Notes (this should create a new layer in the Contents pane)</p></li>
<li><p>Rename the layer (e.g. Estuary Extent Polygon)</p></li>
<li><p>Click on the Edit tab, and choose Create (this should open the Create Features tab)</p></li>
<li><p>Scroll to find the recently created layer and click on it</p></li>
<li><p>Choose your extent by zooming in/out and draw the polygon</p></li>
<li><p>Right click and choose finish</p></li>
<li><p>Edit the symbology to make the polygon transparent</p></li>
</ol></td>
</tr>
<tr>
<td style="text-align: center;">3 </td>
<td>Clip layer to the desired extent</td>
<td><ol type="a">
<li><p>Click on the Analysis tab</p></li>
<li><p>Click Tools</p></li>
<li><p>Search Clip</p></li>
<li><p>This tool allows for an input feature or dataset (the layer you want to clip), clip features (the extent polygon), and an output features of dataset (name of the output layer (e.g. Wastewater_Clip_Nanaimo) – this will be renamed later)</p></li>
</ol></td>
</tr>
<tr>
<td style="text-align: center;">4</td>
<td>Repeat step 3 for each layer</td>
<td></td>
</tr>
<tr>
<td style="text-align: center;">5</td>
<td>Save each layer individually (right click the layer, hover over Sharing, click on Share as Web Layer, a Sharing tab should pop up on the right side of the page, add a summary and tags if necessary, click analyze and if there are no problems, click publish (note whether you want the layers accessible only to you, the organization, or public))</td>
<td></td>
</tr>
<tr>
<td style="text-align: center;">6</td>
<td>Either create a new Web Map in ArcOnline with the same title and add all layers inside or export the map from ArcPro as a Web Map using the Sharing tab</td>
<td></td>
</tr>
<tr>
<td style="text-align: center;">7</td>
<td>Configure the popups for each layer, making sure to save the layer itself (not the entire map) after the code is done</td>
<td>To configure, simply copy and paste the code from the corresponding layer in the full indicator map.</td>
</tr>
</tbody>
</table>
