**There is also a description of each column for the Contaminant Atlas in the Excel sheet under Data Dictionary**

**Purpose:**

The Occurrence Core contains the data extracted from the reports. There is usually a one-to-many relationship between the Event Core and the Occurrence Core where the Occurrence Core has more records than the Event Core.

<table>
<colgroup>
<col style="width: 10%" />
<col style="width: 48%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>Step</strong> </th>
<th style="text-align: center;"><blockquote>
<p><strong>Major Activity</strong> </p>
</blockquote></th>
<th style="text-align: center;"><blockquote>
<p><strong>References, Forms and Details</strong> </p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: center;">1 </td>
<td><ol type="1">
<li><p>Navigate to our shared folder: <a href="https://pacificsalmonfoundation-my.sharepoint.com/:f:/g/personal/psalinasruiz_psf_ca/EtpmRc-zswRJnghvEG1cCB4BIg9CpKGSNxQLfWkr7maYPQ?e=ec04e2">140_ContaminantsAtlas</a></p></li>
<li><p>Select the “Data” Folder</p></li>
<li><p>Open the most recent “ContaminantAtlas_Database_yymmdd”</p></li>
</ol></td>
<td><ul>
<li><p>It is important that the dataset gets updated every 2 weeks. To do so, save the new version with the current date, and move the old version to the “Archived” folder.</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;"></td>
<td></td>
<td><ul>
<li><p>Each site will have its own Occurrence entry, unlike in EventCore</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">2 </td>
<td><blockquote>
<p>Enter fid</p>
</blockquote></td>
<td><ul>
<li><p>“fid” is a unique identifier for each entry made in all 3 Cores. Enter the fid assigned to the sampling site in the Event Core.</p></li>
<li><p>For OccurenceCore_Presence, add _# to each fid so all fids are unique</p></li>
<li><p>For OccurenceCore_Detection, add another _# to each fid</p></li>
<li><p><strong>E.g.</strong> Event fid = 1234</p></li>
</ul>
<p>Presence fid = 1234_3</p>
<p>Detection fid = 1234_3_1</p></td>
</tr>
<tr>
<td style="text-align: center;">3 </td>
<td>Enter eventID associated with that site</td>
<td><ul>
<li><p>Copy from Event Core</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">4</td>
<td>Create occurenceID</td>
<td><ul>
<li><p>OccurenceCore_Presence and OccurenceCore_Detection have different IDs</p></li>
<li><p>There will not be any repeated values in these column (some exceptions)</p></li>
<li><p>Formula is already set up</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">5</td>
<td>Enter verbatimLocality</td>
<td><ul>
<li><p>Verbatim locality is the original textual description of the place as mentioned in the report.</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;"></td>
<td>Enter verbatimSite</td>
<td><ul>
<li><p>Verbatim site is the specific site at which the sample(s) was taken.</p></li>
</ul>
<p>(Make sure ALL sites are included</p></td>
</tr>
<tr>
<td style="text-align: center;">6</td>
<td>Enter dateIdentified</td>
<td><ul>
<li><p>Sampling year</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">7</td>
<td>Enter year</td>
<td><ul>
<li><p>Same as date identified, but with specific formatting for “date” to read in ArcGIS</p></li>
<li><p>Formula is already set up</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">8</td>
<td>Enter latitude and longitude</td>
<td><ul>
<li><p>Make sure the unit are decimal degrees (meters). If the report does not mention lat and long for their stations, use our georeferencing process (<a href="https://pacificsalmonfoundation-my.sharepoint.com/:w:/g/personal/psalinasruiz_psf_ca/EWKY4fJlxBFGntU-Yq9obPEBfO2LY4a_CHAiMbnnkNFdpg?e=Sb2Tbj">130-33</a>) to get a close approximation.</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">9</td>
<td><p>Enter measurementMethod</p>
<p>(Detection only)</p></td>
<td><ul>
<li><p>This is the methodology used by the lab to process the samples.</p></li>
<li><p>Look specifically for the analyzing method</p></li>
<li><p>Enter NA if not listed</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">10</td>
<td><p>Enter Analyzing Lab</p>
<p>(Detection only)</p></td>
<td><ul>
<li><p>Enter NA if not listed</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">11</td>
<td>Enter Media</td>
<td><ul>
<li><p>Material or tissue through which the contaminant was measured</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">12</td>
<td>Enter ContaminantCode</td>
<td><ul>
<li><p>Find in validation</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;"></td>
<td><p>Enter Parameter</p>
<p>(Detection only)</p></td>
<td><ul>
<li><p>Find in validation</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">13</td>
<td><p>Enter Sampled</p>
<p>(Presence only)</p></td>
<td><ul>
<li><p>Whether contaminant was sampled or not. 0 means no and 1 means yes.</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">14</td>
<td><p>Enter Detected</p>
<p>(Detection only)</p></td>
<td><ul>
<li><p>Whether contaminant was detected or not. 0 means no and 1 means yes.</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">15</td>
<td><p>Enter Detection threshold</p>
<p>(Detection only)</p></td>
<td><ul>
<li><p>As reported</p></li>
<li><p>When you are not sure if you have the correct number for the detection threshold, report 1 for Detected and add into Notes what was it could be</p></li>
</ul>
<p>(many times it will be reported as &lt;###, but not say if that means it is under the detection)</p></td>
</tr>
<tr>
<td style="text-align: center;">16</td>
<td>Recorded</td>
<td><ul>
<li><p>Add initials of the person who entered the data</p></li>
</ul></td>
</tr>
<tr>
<td style="text-align: center;">17</td>
<td>Notes</td>
<td><ul>
<li><p>Include information like if there are multiple species of the same organism in that entry See below for example <strong>- Presence</strong></p></li>
<li><p>And if 1 or more of the samples are below the detection threshold (if one or more is above, detected is still = 1) See below for example <strong>- Detection</strong></p></li>
</ul></td>
</tr>
</tbody>
</table>

<img src="140-03_AddingRecordsToOccurrenceCore_240626_media/07a99e079b93dc18fdc679395f9c7a6cf84228cd.png" style="width:6.5in;height:3.48958in" />

<img src="140-03_AddingRecordsToOccurrenceCore_240626_media/689c9f0764d0e797b5e5c9c92c5073485ac45cc8.png" style="width:2.63114in;height:3.44072in" />

Example on how to group organisms within the same sampling site. If there was different species withing the same genus, group them together and make a note that there are multiple species in that sample. (Make sure you do not combine different sampling years)

<img src="140-03_AddingRecordsToOccurrenceCore_240626_media/769ad1ba48d1f1487c1c862e4f7e2010483dbb0f.png" style="width:5.6575in;height:4.55138in" />

Example on how to report detection thresholds for a sample that had multiple thresholds. Since 1 of the 3 was detected (10), report his as detected. In the notes, include that 2 of the 3 samples were not detected and include both 8 and 2 in the detection threshold column.

<img src="140-03_AddingRecordsToOccurrenceCore_240626_media/9afb2ff00d904bc634730eb752d2ac3e18acec0f.png" style="width:7.07143in;height:1.03125in" />
