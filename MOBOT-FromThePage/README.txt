BACKGROUND

These data files are the output of a FromThePage (http://fromthepage.com/) installation
(http://transcribebhl.mobot.org/) that was part of the Purposeful Gaming project
(https://biodivlib.wikispaces.com/Purposeful+Gaming).


FILE FORMAT

Each data file contains the transcriptions for one book, formatted as a fragment of a 
HTML document.  The data elements in each file are contained in <div> and <span>
elements.

To match the transcriptions contained in these data files to their corresponding pages
in BHL, the Internet Archive identifier, page sequence numbers, and page transcriptions
need to be extracted.

Here is an example of the format of the file, with the important data values highlighted:

<body>
   <h2>...</h2>
   <div>....</div>

   <div class="ia_identifier">
      INTERNET_ARCHIVE_IDENTIFIER
   </div>

   <h3>...</h3>
   <div class="pages">

      <div id="page-PAGE_SEQUENCE">
         <h4>...</h4>
         <div class="page-content">
            PAGE_TRANSCRIPTION
         </div>
         ...
      </div>

      <div id="page-PAGE_SEQUENCE">
         <h4>...</h4>
         <div class="page-content">
            PAGE_TRANSCRIPTION
         </div>
         ...
      </div>

      <div id="page-PAGE_SEQUENCE">
         <h4>...</h4>
         <div class="page-content">
            PAGE_TRANSCRIPTION
         </div>
         ...
      </div>

   </div>
   ...
</body>


Each PAGE_SEQUENCE value will be unique within each data file.  In BHL, sequence 
values for a book always start at 1.  In these data files, the starting sequence may be
any value.  The lowest-valued PAGE_SEQUENCE in the file is the first page in the book,
and the highest-values is the last page.  Putting it all together, if the PAGE_SEQUENCE 
values in the above example were 8, 9 and 10, those values would correspond to BHL
sequence values of 1, 2 and 3.

Each PAGE_TRANSCRIPTION value is an XML document containing the text of the 
transcription.  This document needs to be parsed to extract the plain text of the
transcription.

For example, this PAGE_TRANSCRIPTION value...

   <?xml version='1.0' encoding='ISO-8859-15'?>          <page>        <p>F.H. EBELING<br/>(THE PERRY SEED STORE)</p><p>217 WARREN ST.<br/>SYRACUSE, N.Y.<br/>29th ANNUAL CATALOGUE<br/>1899<br/></p>      </page>

... should be parsed to produce this text...

   F.H. EBELING
   (THE PERRY SEED STORE)

   217 WARREN ST.
   SYRACUSE, N.Y.
   29th ANNUAL CATALOGUE
   1899
