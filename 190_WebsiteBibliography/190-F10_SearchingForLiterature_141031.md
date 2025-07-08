---
process_number: 190-F10
title: SearchingForLiterature_141031
author: Unknown
created: Unknown
modified: Unknown
review_period: 3 years
---

Pacific Salmon Foundation
Straight of Georgia (SoG) Literature
Database
(With Ianna's edits)
Description
This document outlines how to update the Straight of Georgia (SoG) Literature Database.
Table of Contents:
• Background
• Provides context for the document.
• Mendeley
• Installation and use of the program used for curating the SoG Literature Database.
• Search strategy
• The terms to search for in each database.
• Inclusion/Exclusion Criteria
• How to identify what citations to keep and to discard.
• Databases
• Where to look for new citations and how to export your findings.
• Logins
• Credentials necessary to complete the work.
Background
For historical context, please refer to the Read_me file in the root folder of "Literature".
The Read_me file also details how the Bibtex file is queried through the literature database web interface.
It is recommended that you read this document through in its entirety before beginning work for the first time.
Statement of Purpose
The SoG Literature Database aims to provide relevant references pertaining to current and historical studies and
information on the Strait of Georgia marine and freshwater ecosystems.
The coverage is broad in scope and includes the following topical areas: physical and chemical oceanography;
hydrography; weather and climate; rivers and streams; flora and fauna (including all marine species, birds and marine
mammals); ecology; biochemistry; water quality; industry and development impacts; hatcheries; aquaculture; human
populations; harvests; and recreational and commercial use, including tourism, boating, fishing, etc.
Importing to Mendeley & Generating a new BibTex file
Mendeley is the citation management software used to curate the SoG Literature Database and build the BibTex file
that is the basis of the online interface available to the public. You should familiarize yourself with how to use
Mendeley before proceeding. Mendeley offers a series of tutorials ➚.

Mendeley will need to be installed locally before proceeding. It is available for all major operating systems including
Linux. Download here ➚.
Login to the PSF account using the credentials in the Login section of this document. Once logged it, the program will
sync with the Mendeley server.
You will also want to install the Mendeley Web Importer ➚. This will facilitate importing references from certain
databases. Mendeley is owned by Elsivier. As such, the databases that have been prioritized to work well with the
Web Importer are those owned by Elsivier. As of the last update to this file, it is not advised to use the Web Importer
for other databases. In addition to the general importing instructions below, each database lists specifics unique to
that database.
Importing
• Before proceeding with any searches, create a new folder in Mendeley for the year/dates being imported.
This simplifies identifying duplicates and the application of the inclusion/exclusion criteria;
• Note: This step only applies if the Web Importer is not being used. While in that folder, go to "File" > "Import"
and select the file format to be imported;
• By importing into this folder, all items are automatically included in "All Documents"
• Once all search results have been imported, de-duplicate records within this folder. To do this:
• Go to "Tools" > "Check for duplicates";
• De-duplication in Mendeley is not perfect. It is advisable to organize records by title after a de-
duplication to ensure that all instances were caught;
• Go through the remaining records to ensure that the content reflects the Straight of Georgia. Off-topic
citations can easily account for more than 40% of retrieved records. Note: Refer to the inclusion/exclusion
criteria to identify off-topic citations;
• Clean up entries with missing or incomprehensible bibliographic information. A search on Google Scholar for a
given title will often identify accurate spelling. For government reports, it may necessary to go back into the
Federal Sciences Library to investigate.
• Clean-up includes:
• All caps are used for article and journal titles - convert these to title case.
• dois are included as a "URL" as opposed to a "Catalog ID". When this is the case, remove the
"http://dx.doi.org/" prefix and place the doi in the appropriate "Catalog ID" field, deleting the
associated url. Leaving the full url will break the auto generation of doi links when interpreted by the
script that generates the html interface for the final BibTex file.
• Dates are missing - locate dates. This often occurs with reports.
• Unusual characters are noticed - replace with proper characters. This often occurs with poorly
encoded accents or other special characters.
• Journal abbreviations are used - replace with the full journal title.
• Once Clean-up is complete, drag and drop the records into the "SoG Library" folder.
• Delete the folder created for the most recent update by right clicking on it and selecting "Remove Folder",
such that the only remaining folders are the "SoG Library" and "Missing Bibliographic Information" folders.
Note: do not delete the files
Generating a new BibTex file
• Note: by default, Mendeley will comment out LaTex characters, which will break urls. It is necessary to go to
Tools > Options > BibTex and uncheck "Escape LaTex special characters" before exporting.

• Select the "All Documents" folder;
• Use Ctrl + A to select all records;
• With all records selected, go to File > Export and save as BibTex;
• Name the file with the convention SOG_YYYY_MM_DD, for example SOG_2015_08_08;
• Forward the file to Nick for uploading to the server. This is most easily done by creating a shared folder in
Google Drive or Dropbox.
• Note: you will need to acquire contact infor for Nick.
Search Strategy
There are 3 search strings reflecting 3 strategies that need be searched for in each database. These are:
• Generic*
• Place specific**
• Fresh water specific
*WorldCat gets only the Generic search string
**The Place specific search string is too long for certain databases. This limitation is noted for each database in its
respective description. When breaking up this search string to accommodate these databases, note that it is
terminated by a NOT string to eliminate duplicate records from the "Generic" search. To facilitate searching, an
example of the string broken into two strings is provided.
Generic
("Strait of Georgia" OR "Georgia Strait" OR "Gulf of Georgia")
Place specific
(("Agamemnon Channel" OR "Baynes Sound" OR "Boundary Bay" OR "Bowen Island" OR "Buccaneer Bay Provincial
Marine Park" OR "Buckley Bay" OR "Burrard Inlet" OR "Bute Inlet" OR "Campbell River" OR "Collinson Marine Park"
OR "Comox Harbour" OR "Copeland Islands Provincial Marine Park" OR "Cortes Island" OR "Cowichan Lake" OR
"Cowichan River" OR "Cowichan River Estuary" OR "Cultus Lake" OR "Decourcy Island" OR "Denman Island" OR
"Departure Bay" OR "Desolation Sound" OR "Discovery Passage" OR "Englishman River" OR "Esquimalt Harbour" OR
"Esquimalt Lagoon" OR "Fanny Bay" OR "Finlayson Arm" OR "fraser river estuary" OR "Fulford Harbour" OR "Gabriola
Island" OR "Galiano Island" OR "Ganges Harbour" OR "Glenora River" OR "Goldstream River" OR "Gulf Islands
National Park" OR "Gulf Islands National Park Reserve" OR "Gulf of Georgia" OR "Harmony Islands Provincial Marine
Park" OR "Haro Strait" OR "Harrison Lake" OR Hernando Island OR "Homfray Channel" OR "Hornby Island" OR "Horne
Lake" OR "Hoskyn Channel" OR "Hotham Sound" OR "Howe Sound" OR "James Island" OR "Jedediah Island" OR "Jervis
Inlet" OR "Kuper Island" OR "Ladysmith Harbour" OR "Lambert Channel" OR "Lasqueti Island" OR "Lewis Channel" OR
"Malaspina Strait" OR "Marina Island" OR "Maurelle Island" OR "Mayne Island" OR "Mill Bay" OR "Millstone River" OR
"Mitlenatch Island" OR "Montagu Channel" OR "Montague Harbour Provincial Marine Park" OR "Moresby Island" OR
"Mudge Island" OR "Nanaimo River" OR "Nanoose Harbour" OR "Narrows Inlet" OR "Nile Creek" OR "Octopus Islands
Marine Park" OR "Okeover Inlet" OR "Oyster River" OR "Pender Island" OR "Pendrell Sound" OR "Pirates Cove Marine
Park" OR "Porlier Pass" OR "Prevost Island" OR "Prince of Wales Reach" OR "Princess Royal Reach" OR "Puntledge
River" OR "Quadra Island" OR "Qualicum Bay" OR "Qualicum National Wildlife Area" OR "Qualicum River" OR "Queens
Reach" OR "Quinsam River" OR "Read Island" OR "Rebecca Spit Provincial Marine Park" OR "Roscoe Bay" OR "Rose
Islets Ecological Reserve" OR "Rosewall Creek" OR "saanich inlet" OR "Sabine Channel" OR "Sabine Channel" OR

"Salmon Inlet" OR "Saltery Bay" OR "saltspring island " OR "San Juan Islands" OR "Saratoga Beach" OR "Satellite
Channel" OR "Saturna Island" OR "Savary Island" OR "Sechelt Inlet" OR "Sechelt Inlets" OR "Shawnigan River" OR
"Shearwater Passage" OR "Sidney Island" OR "Small Inlet Provincial Marine Park" OR "squamish river estuary" OR
"Squitty Bay Provincial Marine Park" OR "Stuart Channel" OR "Sturgeon Bank" OR "Swartz Bay" OR "Texada Island" OR
"Thetis Island" OR "Thormanby Island" OR "Thornborough Channel" OR "Thornhill Creek Provincial Marine Park" OR
"Toba Inlet" OR "Tsolum River" OR "Waddington Channel" OR "Wallace Island Provincial Marine Park" OR "Whaleboat
Island Marine Park" OR "Whiskey Creek") NOT ("strait of Georgia" or "Georgia strait" or "gulf of georgia"))
Fresh water specific
(("Black Creek" OR "Bowen Island" OR "Browns River" OR "Calm Channel" OR "Cameron Lake" OR "Deep Bay" OR
"Desolation Sound" OR "Desolation Sound Provincial Marine Park" OR "Earls Cove" OR "East Redonda Island" OR
"Fulford Harbour" OR "Gambier Island" OR "Ha'thayim Marine Provincial Park" OR "Von Donop" OR "Homfrey
Channel" OR "Jedediah Island Provincial Marine Park" OR "Jervis Island" OR "Little Qualicum River" OR "Mittlenatch
Island Provincial Nature Park" OR "Nelson Island" OR "North Pender Island" OR "North Thormansby Island" OR "Otter
Island" OR "Oyster Bay" OR "Powell Lake" OR "Pryce Channel" OR "Roscoe Bay Provincial Marine Park" OR "Rosewall
Creek" OR "Sabine Channel Provincial Marine Park" OR "Seal Bay" OR "Sechelt Inlets Provincial Marine Park" OR
"Shoal Islands" OR "South Pender Island" OR "South Thormansby Island" OR "Trent River" OR "Victoria Harbour") NOT
("Georgia Strait" OR "Strait of Georgia" OR "Gulf of Georgia"))
If Place specific needs to be broken down, refer to this example:
Place specific 1 of 2
(("Agamemnon Channel" OR "Baynes Sound" OR "Boundary Bay" OR "Bowen Island" OR "Buccaneer Bay Provincial
Marine Park" OR "Buckley Bay" OR "Burrard Inlet" OR "Bute Inlet" OR "Campbell River" OR "Collinson Marine Park"
OR "Comox Harbour" OR "Copeland Islands Provincial Marine Park" OR "Cortes Island" OR "Cowichan Lake" OR
"Cowichan River" OR "Cowichan River Estuary" OR "Cultus Lake" OR "Decourcy Island" OR "Denman Island" OR
"Departure Bay" OR "Desolation Sound" OR "Discovery Passage" OR "Englishman River" OR "Esquimalt Harbour" OR
"Esquimalt Lagoon" OR "Fanny Bay" OR "Finlayson Arm" OR "fraser river estuary" OR "Fulford Harbour" OR "Gabriola
Island" OR "Galiano Island" OR "Ganges Harbour" OR "Glenora River" OR "Goldstream River" OR "Gulf Islands
National Park" OR "Gulf Islands National Park Reserve" OR "Gulf of Georgia" OR "Harmony Islands Provincial Marine
Park" OR "Haro Strait" OR "Harrison Lake" OR Hernando Island OR "Homfray Channel" OR "Hornby Island" OR "Horne
Lake" OR "Hoskyn Channel" OR "Hotham Sound" OR "Howe Sound" OR "James Island" OR "Jedediah Island" OR "Jervis
Inlet" OR "Kuper Island" OR "Ladysmith Harbour" OR "Lambert Channel" OR "Lasqueti Island" OR "Lewis Channel" OR
"Malaspina Strait" OR "Marina Island" OR "Maurelle Island" OR "Mayne Island" OR "Mill Bay" OR "Millstone River" OR
"Mitlenatch Island" OR "Montagu Channel" OR "Montague Harbour Provincial Marine Park") NOT ("strait of Georgia"
or "Georgia strait" or "gulf of georgia"))
Place specific 2 of 2
(("Moresby Island" OR "Mudge Island" OR "Nanaimo River" OR "Nanoose Harbour" OR "Narrows Inlet" OR "Nile
Creek" OR "Octopus Islands Marine Park" OR "Okeover Inlet" OR "Oyster River" OR "Pender Island" OR "Pendrell
Sound" OR "Pirates Cove Marine Park" OR "Porlier Pass" OR "Prevost Island" OR "Prince of Wales Reach" OR "Princess
Royal Reach" OR "Puntledge River" OR "Quadra Island" OR "Qualicum Bay" OR "Qualicum National Wildlife Area" OR
"Qualicum River" OR "Queens Reach" OR "Quinsam River" OR "Read Island" OR "Rebecca Spit Provincial Marine Park"
OR "Roscoe Bay" OR "Rose Islets Ecological Reserve" OR "Rosewall Creek" OR "saanich inlet" OR "Sabine Channel" OR
"Sabine Channel" OR "Salmon Inlet" OR "Saltery Bay" OR "saltspring island " OR "San Juan Islands" OR "Saratoga
Beach" OR "Satellite Channel" OR "Saturna Island" OR "Savary Island" OR "Sechelt Inlet" OR "Sechelt Inlets" OR

"Shawnigan River" OR "Shearwater Passage" OR "Sidney Island" OR "Small Inlet Provincial Marine Park" OR "squamish
river estuary" OR "Squitty Bay Provincial Marine Park" OR "Stuart Channel" OR "Sturgeon Bank" OR "Swartz Bay" OR
"Texada Island" OR "Thetis Island" OR "Thormanby Island" OR "Thornborough Channel" OR "Thornhill Creek Provincial
Marine Park" OR "Toba Inlet" OR "Tsolum River" OR "Waddington Channel" OR "Wallace Island Provincial Marine
Park" OR "Whaleboat Island Marine Park" OR "Whiskey Creek") NOT ("strait of Georgia" or "Georgia strait" or "gulf of
georgia"))
Inclusion/Exclusion Criteria
The inclusion/exclusion criteria for this project defines the scope and nature of references to be included in the SoG
Literature Database. It reflects the desire to accumulate a set of scientific literature reflecting the marine and
freshwater biota and surrounding environment of the Straight of Georgia.
The subject scope in the Statement of Purpose should help to inform the application of the inclusion/exclusion criteria
-further refined to include specific document types - when updating the database.
Inclusion is predominantly defined by the material being:
• Biological, geological, or otherwise environmental in scope.
• This includes marine and freshwater associated wildlife and glacial or sedimentary analyses;
• Marine or freshwater centric.
• This includes material of an enthnobotanical or ethnobiological nature;
• Geographically appropriate. Place names may be duplicated throughout the world; ensure records pertain to
the West Coast;
• Of a scientific nature. This includes the following publication types whether formally published or not:
• Reports, both private and public;
• Theses & dissertations;
• Journal articles;
• Book sections;
• Entire books.
• Works that pertain to land title.
• This includes title negotiation between government and Indigenous peoples.
Exclusion is predominantly defined by the material being:
• Not geographically relevant;
• Not marine or freshwater centric;
• Not biological, geological, or otherwise environmental in scope
• This includes works pertaining to engineering;
• Of an editorial nature;
• A book review;
• Artistic works. This includes:
• Novels;
• Stories;
• Poetry.

Databases
In this section:
• General instructions
• Searching and Exporting
• Databases
• ASFA
• Compendex
• Federal Science Library
• Web of Science Core Collection
• Zoological Record
• CLIR
• WorldCat
General instructions
Searching and Exporting
• Copy and paste the search terms into each respective database.
• Some of the databases are unable to handle the full search strings. If you receive an error or a time
out, break the search string up. At the moment, this includes Compendex and its associated
databases, the Federal Sciences Library, and CLIR
• There are 3 search strings employed for each database (except WorldCat). Consequently there will be
a potential minimum of 3 files of references for each database.
• Proprietary databases will require you to login using the CWL login below.
• Search only the Abstract, Title, and Subject headings. How this is done will differ for each database. Details are
provided below.
• Limit dates to those dates in which you're interested. How this is done will differ for each database. Details are
provided below.
• The inclusion/exclusion criteria may be applied either before or after importing to Mendeley. This is a
personal choice, but its application post importing is simpler in all cases except WorldCat.
• Export the results. How this is done will differ for each database. Details are provided below.
• Search WorldCat last. This is a consequence of how citations are exported. Details are provided below.
• Database interfaces and functionality are regularly updated. Specific details outlined will require updating.
Databases
ASFA ➚
• Search "Abstract", "Publication Title", "Document Title", and "All subjects & indexing". To do this:
• Past the search terms into the first field and select "Abstract" from the dropdown menu and 'OR'
from the other associated dropdown menu;
• Past the search terms into the second field and select "Title" from the dropdown menu and 'OR' from
the other associated dropdown menu;
• Past the search terms into the third field and select "Subject Headings (all)" from the dropdown
menu. It may be necessary to "Add a row".
• Under publication dates, limit dates to those dates in which you're interested and search;
• Select all results;

• Select "Save";
• Export results as .ris
Compendex (GEOBASE & GeoRef) ➚
• Check "Compendex, GEOBASE, and GeoRef" to search all three databases;
• Select "Abstract, Title, and Subject headings" from the dropdown menu and search. Note: Cannot handle the
full search string of "Place specific" names. This will need to be separated into two search strings.
• Using filters on the search results page, limit dates to those dates in which you're interested, and limit the
results.
• Using the Web Importer, paginate through the results (if necessary) and import to appropriate folder. Note:
de-select the option to include pdfs if available. This is important for reasons both of copyright and space
capacity.
• I don't think it's possible to easily obtain data from this database anymore
Federal Science Library ➚
We can no longer search WAVES independently of the Federal Government's other science libraries. Note: The "Place
specific" search string will need to be broken down into 2 search strings to run succesfully.
• Select "Advanced Search"
• Search "Subject Terms", "Title", and "Abstract". To do this:
• Past the search terms into the first field and select "Subject Terms" from the dropdown menu and 'OR'
from the other associated dropdown menu;
• Past the search terms into the second field and select "Title" from the dropdown menu and 'OR' from
the other associated dropdown menu;
• Past the search terms into the third field and select "Abstract" from the dropdown menu.
• Limit dates to those dates in which you're interested and search.
• To export results:
• Add items to "Saved Items" folder;
• View "Saved Items";
• Export to BibTex.
• BibTex didn't work for me, ended up exporting to Zotero and that worked!
Web of Science Core Collection ➚
• Search the "Topic" field only;
• On the results page, use filters to limit to those dates in which you're interested;
• From the dropdown menu, select "Save to Other Formats";
• Input the number of records to export if there is more than one page of results (refer to number of results);
• Export to BibTex.
Zoological Record ➚
• Search the "Topic" field only;
• On the results page, use filters to limit to those dates in which you're interested;
• From the dropdown menu, select "Save to EndNote online" Note: At this time Zoological Record does not
directly output to .ris or BibTex;
• Exporting to EndNote online requires registering an account. No permanent PSF account exists. You will need
to create a new account for the purposes of updating the database. This can then be deleted if you choose
when done;

• Proceed to EndNote online following the links at the top of the page from within Zoological Record;
• Under "Format" select "Export references";
• Select "All references in my Library";
• Export to .ris. Note: Exporting to BibTex will not export abstracts;
• Return to "My References" and delete all references before proceeding.
CLIR: Cross-linked Information Resources ➚
Note: CLIR is restricted to 250 characters. The search strings will need to be broken up accordingly, making this search
more onerous than the others. The search is quite buggy. Also, there is no embeded bibliographic metadata, so
results will need to be manually entered into Mendeley. NOTE: Use Advanced Search, use an online character
counter, put your search in the "Keyword" box with NO brackets, add your dates by year.
• From the landing page, select "Public access to CLIR";
• Check the option "Search for all words";
• Leave all e-Libraries selected;
• There is no date selection feature;
• Create entries manually in Mendeley.
WorldCat ➚
Note: In WorldCat search only the "Generic" search string.
• In the dropdown menu for libraries to search, select "Libraries Worldwide";
• On the results page, limit to those dates in which you're interested;
• There is no bulk export of citations available;
• Compare titles of documents of interest with those already in Mendeley. The majority of the records are
captured elsewhere;
• Export individual citations of interest using the "Cite/Export" option on each individual record page;
• Export to EndNote/Reference Manager, which will save to .ris.
Logins
UBC Campus Wide Login (for licensed database access)
• Username: isobelp
• Password: Datacentre10!
• DUO Password: 836139
Mendeley
• Username: sogdatacentre@gmail.com
• Password: Datacentre!
RefWorks (Obsolete as of 2017, kept here only for historical reference)
• Username: pearsalli@shaw.ca
• Password: Georgia
• Group code: ubclibref