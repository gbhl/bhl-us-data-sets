BACKGROUND

These data files are the output of Science Gossip ( http://www.sciencegossip.org/ ), 
which is collaboration between Zooniverse ( https://www.zooniverse.org/ ) and the 
Biodiversity Heritage Library (BHL).

The Zooniverse is a collection of web-based citizen science projects that use the 
efforts of volunteers to help researchers deal with the flood of data that confronts 
them.  Science Gossip is one of these sites.

Science Gossip is born from a collaboration between an Arts and Humanities Research 
Council project in the UK, called ‘Constructing Scientific Communities: Citizen 
Science in the 19th and 21st Centuries’ (ConSciCom) and the Missouri Botanical 
Garden who are providing content from the Biodiversity Heritage Library.

The ConSciCom project is investigating the role of naturalists and ‘amature’ science 
enthusiasts in the making and communication of science in both the Victorian period 
and today. Historians at the Universities of Leicester and Oxford are investigating 
the particular roles of the periodical press in the nineteenth century as an arena 
in which citizen scientists of the past participated in scientific research. 
Periodicals and books of the Victorian era were heavily illustrated, but little is 
known about who made the illustrations and how they ended up in print. The data 
created by tagging illustrations in Science Gossip and adding artist and engraver 
information will have a direct impact on the research of historians who are trying 
to figure out why, how often, and who made images depicting a whole range of natural 
sciences in the Victorian period.  It is this data that is contained in the data 
files found here.

The data files were downloaded from http://explore.sciencegossip.org/groups.


FILE FORMAT

The data file names follow this pattern:

	<ZOONIVERSEID>-<BHLTITLEID>.csv

	where 	ZOONIVERSEID is the identifier of the title in the Zooniverse system.
				Access the title in Zooniverse using this URL:
				http://explore.sciencegossip.org/groups/<ZOONIVERSEID>
			BHLTITLEID is the identifier of the title in BHL
				Access the title in BHL using this URL:
				http://www.biodiversitylibrary.org/bibliography/<BHLTITLEID>

Each data file is a comma-separated value (CSV) file containing data for a single BHL 
title.  As each BHL title may include one or more individual volumes, each data file 
may contain data for one or more books.

Each row in a data file contains values for one type of classification assigned to a 
single page in a book.  Some types of classifications are keywords, inscriptions, 
species names, and illustration types.  So, for example, a single row in a data file 
may contain a list of species names that appear on a page.

Each row in a data file contains ten columns.  The first row in each file contains 
the column names.  See the following section in this file for information about the 
data found in each column.  


COLUMN DEFINITIONS

Zooniverse ID - Identifier of the page in the Zooniverse system.  Use the following URL
	to view the page details on the Zooniverse web site:
	http://explore.sciencegossip.org/subjects/ASC0000048, where ASC0000048 is the 
	Zooniverse identifier.

Classification count - The number of Zooniverse users that have classified the page.

Page ID - Identifier of the page in BHL.  Use the following URL to view the page in BHL:
	http://www.biodiversitylibrary.org/page/1000, where 1000 is the BHL page 
	identifier.

Volume - Volume number for the page.  May include other information.  For example,
	a value of "v. 4 1842" includes the volume "4" and year "1842".

Page - Pagination information for the page.  For example, "Page 1", "Plate VI".

Year - Year of publication for the page.

Image scale - A value that indicates the amount that the original BHL source image 
	was scaled for use in Zooniverse.  To convert the coordinate values (see the Coords 
	column) so that they will map onto the BHL source image, divide them by the "Image 
	scale" value.

Type - Describes the type of classification data collected for the page.  Possible 
	values include:

	Page keywords
	inscription (transcription of text on the page)
	contributor
	species (scientific or common names that describe some element of the page)
	drawing
	chart
	map
	photograph
	
Coords - Coordinates of the page element being classified.  Six coordinates are 
	listed.  The first two apply to text elements like "inscription" and "species".  
	The last four apply to graphical elements like "drawing", "chart", "map", and 
	"photograph".  In all cases, the origin (0,0) is the upper left corner of the 
	page image. When the first two coordinates are specified, they represent the 
	(x,y) position of the page element being classified.  When the last four 
	coordinates are specified, the first of those is the top position of the 
	bounding box around the element being classified and the second is the left 
	position of the bounding box.  The third coordinate is the width of the bounding 
	box, and the fourth coordinate is the height of the bounding box.  Put another 
	way, the coordinates array contains the following: 
	[x, y, top, left, width, height]

Value - Value of the classification.  Typically, this is a structured list of values.  
	Note that values like tree, trees, Tree, and Trees are all considered to be 
	distinct values.

	The format of the value column is
	{"KEY1"=>["VALUE1.1","VALUE1.2"],"KEY2"=>["VALUE2.1","VALUE2.2"]}
	where KEY identifies the classification subtype, and VALUE is a specific value.

	Following are examples of values for several different Types.

	Type: chart
	Value: {"keywords"=>["water-glass", "Potash: waterglass", "potash water-glass", "quartz", "potash", "charcoal"]}
	Explanation:  The Value field contains six "keywords" that have been assigned to 
		the chart.

	Type: contributor
	Value: {"name"=>["E. J. Lowe", "E J Lower", "E.J. Lowe", "E.J.Lowe"], "role"=>["other", "illustrator"]}
	Explanation:  The Value field contains four different spellings of the contributor 
		"name", and two contributor "roles".

	Type: drawing
	Value: {"keywords"=>["Symbol"]}
	Explanation:  The Value field contains one "keyword" that has been assigned to the 
		drawing.

	Type: inscription
	Value: {"text"=>["Fig. 1--Petal of Common Poppy", "Petal of Common Poppy", "Petal of the Common Poppy"]}
	Explanation:  The Value field contains four different values for the "text" of the 
		inscription.

	Type: map
	Value: {"keywords"=>["earthquake", "globe", "world map", "tectonics", "volcano", "world", "principal lines of volcanic and earthquake phenomena"]}
	Explanation:  The Value field contains seven "keywords" that have been assigned to 
		the map.

	Type: Page keywords
	Value: ["sponges", "sponge", "physiology", "marine zoology", "history", "seashore", "porifera", "ocean", "coral", "biology", "Fossils ", "anatomy"]
	Explanation:  The Value field contains eleven keywords that have been assigned to 
		the page.  Note that there is no subfield in this Value field.

	Type: photograph
	Value: {"keywords"=>["venus", "planet", "Planets"]}
	Explanation:  The Value field contains three "keywords" that have been assigned to 
		the photograph.

	Type: species
	Value: {"common"=>["December Moth", "moth", "Butterfly"], "scientific"=>["Pacilocampa Populi", "Paecilocampa Populi", "", "Poecilocampa Populi"]}
	Explanation: The Value field contains three "common" names for the species, and 
		four "scientific" names for the species (one is blank).


IMPORTANT NOTE

Two of the data sets (GSC0000007-45236.csv and GSC000000a-51125.csv) contain incorrect 
Page ID values.  The files GSC0000007-45236-CORRECTED.csv and 
GSC000000a-51125-CORRECTED.csv map the Zooniverse IDs in those data sets to the correct 
Page ID values.

For example, the rows in the file GSC0000007-45236.csv with Zooniverse ID ASC0000y54 have
Page ID 12536652.  That Page ID is incorrect.  GSC0000007-45236-CORRECTED.csv contains
a row for Zooniverse ID ASC0000y54 with Page ID 12536653, which is the correct value.
