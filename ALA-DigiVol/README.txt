BACKGROUND

These data files are exported from DigiVol (https://volunteer.ala.org.au/), which
was used to transcribe journals and diaries as part of the Purposeful Gaming 
project (https://biodivlib.wikispaces.com/Purposeful+Gaming).


FILE FORMAT

Each data file is a comma-separated value (CSV) file containing the transcriptions 
for one book.

Each row contains the transcription for a single page.


COLUMN DEFINITIONS

To extract the transcriptions contained in these data files and match them to their 
corresponding pages in BHL, only two of the columns are relevant.

taskID - NA

validationStatus - NA

transcriberID - NA

validatorID - NA

externalIdentifier - The filename of the page image, containing both the Internet Archive 
	identifier for the book and the sequence number of the page.

	Filename format: IAIDENTIFIER_SEQNO.jpg

	where 	IAIDENTIFIER is the Internet Archive identifier for the book
		SEQNO is the sequence nubmer of the page

	Given IAIDENTIFIER and SEQNO, the BHL page to which the transcription
	applies can be easily located.

exportComment - NA

dateTranscribed - NA

dateValidated - NA

individualCount - NA

institutionCode - NA

occurrenceRemarks - The transcription of the page.  Line breaks are encoded as \n.
	
sequenceNumber - NA

transcriberNotes - NA

validatorNotes - NA


