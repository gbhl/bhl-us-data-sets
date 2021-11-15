### BACKGROUND

These data files accompany an internship research project between McGill University and the Biodiversity Heritage Library, as described by Lidia Ponce de la Vega in a two-part blog series. See https://blog.biodiversitylibrary.org/2021/11/understanding-bhl-through-metadata-patterns-of-bio-diverse-knowledge-production.html and https://blog.biodiversitylibrary.org/2021/11/geopolitics-of-metadata-knowing-panama-through-biodiversity-heritage-library.html.
This project constitutes an analysis of metadata patterns in materials about Latin America in BHL's collection to identify shortcomings in the equitable representation of materials about Latin America, to recognize and counteract biases in the presence and importance of sites of knowledge production in the Global South versus the Global North, and to inform decolonizing strategies and policy. 
Data employed in this project were downloaded from https://www.biodiversitylibrary.org/data as of July 1st, 2021.

### FILE FORMAT

Each data file is a Microsoft Excel spreadsheet (.xlsx) containing metadata categories for materials in BHL's collection that include one or more subjects related to Latin America in their subject lists. See the following sections in this file for information about the data found in each file.
Each row in a data file contains between two and thirteen columns. The first row in each file contains the column names. See the following sections in this file for information about the data found in each column. 
Each visualization file is a portable network graphics (PNG) file showing the visual of a portion of the analyses performed in this project. See the following sections in this file for information about the nature of and data used for each visualization.

### FILE DESCRIPTION

All acronyms for subset names are indicated in parentheses in the next section of this file. 

SUB Lists.xlsx - XLSX file containing listed subjects per TitleID for all records (146806) that were part of BHL's collection as of July 1st, 2021.

Data files - XLSX files belonging to one of the following groups:
- Metadata subsets - XLSX files including full metadata details for the selected materials. The names of these files follow one of these two patterns:

	- \<Subset acronym\>.xlsx
		OR
	- \<Subset acronym\> - Unique.xlsx

		When the second pattern is used, only unique title IDs for the selected subject are included, i.e. works in volumes, issues, and/or numbers appear as a single record under their shared title ID.

- Subject lists - XLSX files including only listed subjects per TitleID for the selected materials. The names of these files follow this pattern:
	- \<Subset acronym\> - SL.xlsx

- Word frequencies - XLSX files including only the most frequent words in each subject list for the selected materials. The names of these files follow this pattern:
	- \<Subset acronym\> - WF.xlsx

Visualizations - PNG files presenting visuals for metadata statistics, co-occurrence networks, or hierarchical clustering of each subset. Depending of the nature of the visualization, the names of these files follow one of the following patterns:

- Holding institution counts: \<Subset acronym\> HI.png
- Place of publication counts (graphs): \<Subset acronym\> PP - G.png
- Place of publication counts (map): \<Subset acronym\> PP - M.png
- Language counts: \<Subset acronym\> LANG.png
- Subject counts: \<Subset acronym\> SUB.png
- Year counts: \<Subset acronym\> YR.png
- Language counts per holding institution: \<Subset acronym\> LANG-HI.png
- Language counts per place of publication: \<Subset acronym\> LANG-PP.png
- Language counts per included subject: \<Subset acronym\> LANG-SUB.png
- Language counts per year of publication: \<Subset acronym\> LANG-YR.png
- Subject counts per holding institution: \<Subset acronym\> SUB-HI.png
- Subject counts per place of publication: \<Subset acronym\> SUB-PP.png
- Year counts per place of publication: \<Subset acronym\> YR-PP.png
- Co-occurrence networks: \<Subset acronym\> CON.png
- Hiearchical clustering: \<Subset acronym\> HC.png
	
When the name includes the indication - Unique, only unique title IDs for the selected subject were considered.

### SUBSETS DESCRIPTION

- Greater Regions (GR) subset - Incorporates all BHL records (4465) that include at least one of the following subjects: Latin America, Central America, South America, West Indies. 
- Latin American Countries (LAC) subset - Incorporates all BHL records (6801) that include the name of at least one Latin American country (except Mexico): Argentina, Belize, Bolivia, Brazil,  British Guiana, Chile, Colombia, Costa Rica/Costa-Rica, Ecuador, El Salvador, French Guiana, Guatemala, Guiana/Guyana, Honduras, Nicaragua, Panama, Paraguay, Peru, Surinam/e, Uruguay, Venezuela.
- Mexico (MEX) subset - Incorporates all BHL records (2995) that include at least one of the following subjects: Mexico; Mexico, North; Mexico, Northern.
- Indigenous Peoples – General (IP-G) subset - Incorporates all BHL records (1052) that include at least one of the following subjects: Indians of Central America, Indians of Mexico, Indians of South America, Indians of the West Indies, Aztecs, Incas. 
- Indigenous Peoples – Specific (IP-S) subset - Incorporates all BHL records (135) that include at least one of the following subjects: Carib Indians, Choco Indians, Cuna Indians, Diaquita Indians, Goajiro Indians, Huichol Indians, Kickapoo Indians, Mapuche Indians, Mayas, Mayoruna Indians, Mojo Indians, Shipibo-Conibo Indians, Taino Indians, Tairona Indians, Tarahumara Indians, Yahgan Indians.
- West Indies (WI) - Contains all unique IDs (228) that include the subject West Indies. 
- Central-Latin-South America (CLS) - Contains all unique IDs (710) that include at least one of the following subjects: Central America, Latin America, South America. 
- Central American Countries (CAC) - Contains all unique IDs (485) that include the name of at least one Central American country: Belize, Guatemala, Honduras, Nicaragua, Costa Rica, Panama, El Salvador.
- South American Countries (except Brazil) (SAC)- Contains all unique IDs (1221) that include the name of at least one South American country (except Brazil): Argentina, Bolivia, Colombia, Chile, Ecuador, Guyana, (French) Guiana, Paraguay, Peru, Surinam/Suriname, Uruguay, Venezuela.
- Brazil (BR) - Contains all unique IDs (543) that include the subject Brazil.
- Mexico (MEX SUB) - Contains all unique IDs (917) that include the subject Mexico.
- Panama (PAN) - Contains all unique IDs (185) that include the subject Panama.

### COLUMN DEFINITIONS

- TitleID - Identifier of each included material as determined by BHL. 
- Title - Full title of each included material.
- Author - Full name of the author(s) and years of birth and death (when appropriate).
- Holding Institution - Name of the institution that contributes the material to BHL.
- Year - Year of publication of each included material.
- StartYear - Year of first volume/issue publication of each included material (for volumes and periodicals).
- EndYear - Year of final volume/issue publication of each included material (for volumes and periodicals).
- Full Publication Details - Known publication details exactly as they appear in each included material and/or in BHL's database. 
- Place of Publication - Place of publication of each included material extracted and cleaned from the "Full Publication Details" column. 
- Latitude - Latitude coordinate for the place of publication of each included material, as appears in the "Place of Publication" column. 
- Longitude - Longitude coordinate for the place of publication of each included material, as appears in the "Place of Publication" column.
- Language - Language code for each included material. 
- Includes Subject - Subject that appears in each included material for it to be selected as part of a specific subset. 
- Location of Indigenous group - Geographical location (countries) of the Indigenous group(s) included as subject.
- TitleURL - BHL URL for each included material. 
- Listed subjects - Complete list of subjects for each included material as they appear in BHL's database.
- Words - Most frequent words in a subject list subset, from most frequent to least frequent. 
- POS - Part of speech of each word in a subject list subset.
- Frequency - Frequency counts for each word in a subject list subset. 

### VISUALIZATIONS DESCRIPTION

- Counts graphs - PNG visualization of counts of one or two metadata categories of records included in each subset. All graphs were generated on Tableau.
- Co-occurrence networks - PNG visualization of the relationships between subjects included in each subset based on word frequency and co-occurrence counts. All co-occurrence networks were generated on KH Coder 3.
- Hierarchical clustering - PNG visualization of the relationships between subjects included in each subset based on word distance. All hierarchical clusters were generated on KH Coder 3.

### IMPORTANT NOTE ON THE PAN SUBSET

Two data files for unique IDs in the PAN subset are included. Data in the second file (PAN - Unique - No missing fields.csv) have been cleaned to reduce the number of missing fields in these records. 
