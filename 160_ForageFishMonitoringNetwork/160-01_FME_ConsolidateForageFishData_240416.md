**Purpose:**

This document describes how to use FME to create a consolidated dataset that takes source data from multiple organizations and combines them to one dataset with 15 preset fields. The purpose of this consolidated dataset is to assist the efforts of the Strait of Georgia Forage Fish Monitoring Network by uniting the data into a simplified format.

Dependencies: 1) FME Workbench 2) Excel dataset forage fish monitoring inputs from various organizations (MABBRI, SeaWatch, PODS, Peninsula Streams Society, Project Watershed) in the same format as when they were available through the Strait of Georgia Data Centre as of March 2021.3) ShoreZone Unit Lines as available though: http://soggy.zoology.ubc.ca:8080/geoserver/ows?service=wfs&version=2.0.0&request=GetCapabilities

<table>
<colgroup>
<col style="width: 17%" />
<col style="width: 50%" />
<col style="width: 31%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Step</strong></th>
<th><strong>Major Activity</strong></th>
<th><strong>References, Forms and Details</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;">1</td>
<td>Open <em>ff-consolidation-fme-workflow.fmw</em></td>
<td><p>Required FME Workbench with active license.</p>
<p>Workflow created in FME Workbench 2020.0</p></td>
</tr>
<tr>
<td style="text-align: center;">2</td>
<td><p>Add Readers for each of the datasets from the source organizations.</p>
<p>If data has been updated beforehand and uploaded to SoGDC GeoNetwork in XLSX format:</p>
<ul>
<li><p>Set the Reader Format as <strong>Mircrosoft Excel</strong></p></li>
<li><p>From the Marine Data BC GeoNetwork forage fish child record containing the XLSX (e.g. “Pacific Sand Lance Data for Pender Harbour &amp; Thormanby Island”), right-click the link to the XLSX and open in a new window. Copy the URL from the newly opened window and paste it in the ‘Dataset’ box of the FME Reader. Alternatively, fill the dataset box with the file path to a downloaded version of the XLSX.</p></li>
<li><p>Press OK to run the FME Reader.</p></li>
</ul></td>
<td></td>
</tr>
<tr>
<td style="text-align: center;">3</td>
<td><p>Connect the results of running the Reader to the associated Bookmark for the organization. This is accomplished by clicking and dragging the arrow on the right side of the Reader to the arrow on the left side of the input Transformer for the organizational Bookmark.</p>
<p>In some cases, the comments in the FME workflow may advise differently as to which Transformers to connect the Reader to (e.g. if multiple sheets exist within a dataset)</p></td>
<td>-The FME Workbook has had comments added advising as to where to place the Readers.</td>
</tr>
<tr>
<td style="text-align: center;">4</td>
<td><p>At the far right of the FME worklow, add a Writer of your choice. For example, select PostGIS and:</p>
<p>-add your desired connection information.</p>
<p>-select ‘Parameters…’🡪’Advanced’ 🡪Change ‘Features Per Transaction to 10000 (or higher if necessary)</p>
<p>*for ‘Table Definition’ change from ‘Copy from Reader…’ to ‘Automatic…’</p>
<p>Press OK</p></td>
<td>Many output formats are available, PostGIS or CSV are recommended</td>
</tr>
<tr>
<td style="text-align: center;">5</td>
<td><p>If outputting as a PostGIS table, in the pop-up that appears, enter a table name of your choosing.</p>
<p>Press OK</p></td>
<td>Alternatively, it may be a CSV file name, shapefile name or any number of other options depending on what format was selected in the previous step</td>
</tr>
<tr>
<td style="text-align: center;">6</td>
<td>If outputting a PostGIS table, once the Writer has appeared drag the arrow from ‘FeatureHolder_2’ to the arrow on the left side of the Writer.</td>
<td>The step is the same for other output formats as well.</td>
</tr>
<tr>
<td style="text-align: center;">7</td>
<td>If outputting a PostGIS table, click the gear symbol at the top of the writer, go to ‘Format Attributes’, switch ‘Attribute Definition’ to ‘Manual’ and change data types as desired for input into the PostGIS table.</td>
<td><p>In testing the workflow, PostGIS data types were set to <strong>varchar (width of 50)</strong> for all fields except for:</p>
<p>-objectid = oid</p>
<p>-datetime = timestamptz</p>
<p>-latitude = float8</p>
<p>-longitude = float8</p>
<p>-attribution = varchar (width of 500)</p></td>
</tr>
<tr>
<td style="text-align: center;">8</td>
<td>Click Run in the top left of the Workbench</td>
<td></td>
</tr>
<tr>
<td style="text-align: center;">9</td>
<td>Fix any error messages that arise</td>
<td>This Workbench is dependent on data sources being input in certain formats. If the formats change, there is a high likelihood the Workbench will need to be updated.</td>
</tr>
<tr>
<td style="text-align: center;">10</td>
<td><p>Ensure the output table is of the desired quality. Things to check for:</p>
<ul>
<li><p>Does the # of input rows = the # of output rows</p></li>
<li><p>Does the data map correctly in a GIS (coordinate system is EPSG: 4326)</p></li>
<li><p>Do the datetime values match between the inputs and the output</p></li>
<li><p>Do the ‘egg’ outputs match the inputs</p></li>
<li><p>When mapping phyident, does everything appear as expected (I.e. no obvious mismatches)</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>
