.. include:: partials/substitutions.rst

*****************
MGnify Services
*****************

In the presentation we will cover:

- Overview of MGnify annotation pipeline
- Taxonomic assignment
- Functional characterisation
- Pathways/systems
- Other MGnify services
- API Overview

MGnify hands-on exercises
##################################

For this session we will look at some of the data and analyses that are available from MGnify. We will navigate the resource, try out different ways to search for interesting samples/studies, and then investigate the analysis results that are available.

Browsing MGnify
****************

From the MGnify front page (https://www.ebi.ac.uk/metagenomics/) you can see various options to browse the data. There are quick links to the various data-types (e.g. amplicon, assembly, metagenomes, etc) we support, as well as a subset of the biomes that the data covers.

|action| Click on the "wastewater" biome icon.

|question| How many studies does MGnify hold that relate to wastewater?

|question| How many samples does that relate to?

|action| From the sample list, filter for sample "ERS1215575", select it and take a look at the metadata available.

|question| Do you know the exact location of where the sample was taken?

|question| What are the lat/long co-ordinates?

|question| Follow the link to the BioSamples record, can you find any more information about the location of the sample?

|action| From the tabs in the header bar, select **Text search**, and then select **Samples** below the search box. There are a number of metadata fields available to allow you to filter for a sample of interest to you. Not all are relevant to all samples. 
Within the hierarchy of biomes, navigate to environmental>aquatic>lentic. You should see 92 samples. Now select the depth filter.

|question| How many lentic samples have depth data associated with them?

|question| Using the sliders, can you identify a sample of a lentic water system from a depth between 25-50m?

MGnify assembly analysis
**************************

Now we will look at some assembly data that has been analysed by MGnify. 

|action| Search for **MGYS00003598**, and go to this study page. This is a large study where MGnify have assembled the raw reads from an existing public study. The list of assemblies is shown at the bottom of the study page.

|question| How many assemblies are included in this study?

|action| Now, search for the analysis **MGYA00510849**. You can use the text search to find this accession. Have a look at the information within the **Quality control** tab.

|question| How many contigs are included in this analysis?

|question| What length is the longest contig in this dataset?

|action| Click on the **Taxonomic analysis** tab and examine the phylum composition in the graphs and the krona plot.

|question| What proportion of the total LSU rRNA predictions are eukaryotic? 

|question| What proportion of the bacterial predictions are proteobacteria?

|action| Click on the **Functional analysis** tab. The top part of this page shows a sequence feature summary, showing the number of contigs with predicted coding sequences (pCDS), the number of pCDS with InterPro matches, etc.

|question| How many predicted coding sequences (pCDS) are in the assembly? 

|question| How many pCDS have InterProScan hits? 

|action| Scroll down the page to the InterPro match summary section.

|question| How many different InterPro entries are matched by the pCDS? 

|question| Why is this figure different to the number of pCDS that have InterProScan hits? 

|action| Click on the **GO Terms** sub-tab. This shows a summary of the most common GO terms annotated to the pCDS as both bar charts, and pie charts.

|question| What are the top 3 biological process terms predicted for the pCDS from this assembly? 

|action| Have a look at the information in the **Pfam** and **KO** (KEGG orthologue) sub-tabs.

|action| Click on the **Pathways/Systems** tab. Have a look at the data reported in the 3 sub-tabs: KEGG Module, Genome Properties, and antiSMASH.

|question| How many KEGG modules are reported for this assembly? 

|question| How many of these are 100% complete (i.e. all of the constituent KOs are found)? 

|question| How many Genome Properties of the category **DNA handling**, are found within this assembly? 

|question| What is the most common class of biosynthetic gene cluster found in this assembly?

|question| How many non-ribosomal peptide synthetase gene clusters are identified by antiSMASH in this assembly?

|action| Click on the **Contig Viewer** tab. Load the data for the 4th contig in the list by clicking on the contig name (ERZ501066.4-NODE-4-length-276957-cov-33.799655). This contig will now be loaded into the viewer.

|question| How long is this contig? 

|question| The longest pCDS in the contig appears to start at 202339. What protein is coded for? 

|question| Looking at the antiSMASH annotations, where within the contig do any transport-related genes fall? 

|action| Zoom into that region to see the predicted regions in more detail. Have a look at the information about the various transport-related genes. 

|question| What region of the contig is predicted to code for a major facilitator transporter? 

|info| There are lots of different visualisation options available within the contig viewer. Take some time now to investigate the various options, and play about with it by looking at a few different contigs and the anotations they contain.

MGnify sequence search
**********************

Now we will have a look at the database of proteins identified by MGnify. 

|action| Click on "Sequence search" from the tabs at the top of the page. 

This will open a HMMER search page specific for MGnify. (For more information about the HMMER suite of tools see the HMMER website https://www.ebi.ac.uk/Tools/hmmer/)

|action| Copy and paste the protein sequence below into the sequence search box at the top of the page, and click "submit".

::

GEFWHWTNLLHFILVGLAGGMAFLTALLHLKGHPEARRYTLWALGLIALDLFVLWAESPARFRFTHV
WLFLSFHPTSPIWWGSWGLALSVSAGLLYLGKGPSKPLAWGLLAFSLVALAYPGMALAVNLNRPLWN
ALLAGLFPLTALVLGLGVAVLMKSSWALYPLRILLGASLFLAFLYPFTLTLEARGHLWEEGGVLYGL
FLALGLGAFGKESLAPWAAFLAAAGLRALLVAVGQWQG

|question| How many query results are significant? (i.e. above the red cut-off line)

|action| Click on the "Customise" button at the top right of the results table, and select to make "Run and sample IDs" column visible and click "Update". Have a look at the sample data for some of the runs listed in the results (for example the top match result).

|question| We know that the protein belongs to IPR032796 - Polysulfide reductase, we looked for this before hand using InterProScan (https://www.ebi.ac.uk/interpro/search/sequence/). Looking at the samples included in the significant results, does it make sense that the example sequence was from this protein family?.

API
***

An `API <https://en.wikipedia.org/wiki/API>`_ ("Application programming interface") is how your scripts (e.g. Python or R) can talk to the MGnify database.

For this section of the practical session we will use a Jupyter Notebook.

.. include:: partials/jupyter.rst

Today's Notebook is "Day 2".