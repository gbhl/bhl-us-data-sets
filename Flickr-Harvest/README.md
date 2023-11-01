### BACKGROUND

BHL has uploaded over 300,000 images to Flickr (https://www.flickr.com/photos/biodivlibrary/sets/).  BHL and Flickr users have added over 2,000,000 tags and notes to these images on the Flickr platform.

Periodically, BHL harvests those tags and notes and stores them in a database.

Contained in these files are the Flickr tags and notes, combined with additional BHL metadata that is associated with each page image.  The metadata is formatted as JSON.  It has been separated into four files due to the total combined size of the dataset.

### EXAMPLE

Every record in the files will be formatted similar to this example.

```
{    
  "Pages": [    
    {        
      "TitleID": 46288,
      "ItemID": 100215,
      "PageID": 32127307,
      "Title": "The Cactaceae : descriptions and illustrations of plants of the cactus family",
      "Authors": [
        {
          "AuthorID": 282,
          "Role": "Main Entry -- Personal Name (MARC 100)",
          "Name": "Britton, Nathaniel Lord,",
          "FullerForm": "",
          "StartDate": "1859",
          "EndDate": "1934"
        },
        {
          "AuthorID": 234478,
          "Role": "Added Entry -- Personal Name (MARC 700)",
          "Name": "Rose, J. N.",
          "FullerForm": "(Joseph Nelson),",
          "StartDate": "1862",
          "EndDate": "1928"
        }
      ],
      "PublicationStartDate": 1919,
      "PublicationEndDate": 1923,
      "ItemStartYear": "1919",
      "ItemEndYear": "1923",
      "HoldingInstitution": "New York Botanical Garden, LuEsther T. Mertz Library",
      "SourceIdentifier": "cactaceaedescri03brit",
      "StartVolume": "3",
      "EndVolume": "",
      "StartIssue": "",
      "EndIssue": "",
      "Sponsor": "The LuEsther T Mertz Library, the New York Botanical Garden",
      "Language": "English",
      "LicenseUrl": "",
      "Rights": "https://www.biodiversitylibrary.org/permissions/",
      "CopyrightStatus": "Public domain. The BHL considers that this work is no longer under copyright protection.",
      "FlickrURL": "https://www.flickr.com/photos/61021753@N02/8569078748/",
      "PhotoID": "8569078748",
      "DateImageAddedToFlickr": "2013-03-18T09:42:52.993",
      "PageTypes": [
        {
          "TypeName": "Illustration"
        }
      ],
      "FlickrTags": [
        {
          "IsMachineTag": 0,
          "TagValue": "Mertz Library, The New York Botanical Garden",
          "FlickrAuthorID": "61021753@N02",
          "FlickrAuthorName": "BioDivLibrary",
          "CreationDate": "2020-05-09T03:46:30.440"
        },
        {
          "IsMachineTag": 0,
          "TagValue": "Mary Emily Eaton",
          "FlickrAuthorID": "61021753@N02",
          "FlickrAuthorName": "BioDivLibrary",
          "CreationDate": "2020-05-09T03:46:30.457"
        },
        {
          "IsMachineTag": 1,
          "TagValue": "artist:name=Mary Emily Eaton",
          "FlickrAuthorID": "61021753@N02",
          "FlickrAuthorName": "BioDivLibrary",
          "CreationDate": "2020-05-09T03:46:30.457"
        },
        {
          "IsMachineTag": 0,
          "TagValue": "Q1287986",
          "FlickrAuthorID": "61021753@N02",
          "FlickrAuthorName": "BioDivLibrary",
          "CreationDate": "2020-05-09T03:46:30.457"
        },
        {
          "IsMachineTag": 1,
          "TagValue": "illustrator:wikidata=Q1287986",
          "FlickrAuthorID": "61021753@N02",
          "FlickrAuthorName": "BioDivLibrary",
          "CreationDate": "2020-05-09T03:46:30.457"
        }
      ],
      "FlickrNotes": [
        {
          "NoteValue": "taxonomy:binomial=&quot;Echinocereus pentalophus&quot;",
          "FlickrAuthorID": "126912357@N06",
          "FlickrAuthorName": "siobhan leachman",
          "CreationDate": "2017-12-20T19:44:26.460"
        },
        {
          "NoteValue": "taxonomy:trinomial=&quot; Echinocereus reichenbachii var. fitchii&quot;",
          "FlickrAuthorID": "126912357@N06",
          "FlickrAuthorName": "siobhan leachman",
          "CreationDate": "2017-12-20T19:44:26.463"
        },
        {
          "NoteValue": "taxonomy:genus=Echinocereus",
          "FlickrAuthorID": "126912357@N06",
          "FlickrAuthorName": "siobhan leachman",
          "CreationDate": "2017-12-20T19:44:26.467"
        }
      ],
      "ScientificNames": [
        {
          "NameFound": "Echinocereus pentalophus",
          "NameConfirmed": "Echinocereus pentalophus (DC.) Engelm. ex Haage",
          "NameCanonical": "Echinocereus pentalophus"
        },
        {
          "NameFound": "Echinocereus",
          "NameConfirmed": "Echinocereus Engelm.",
          "NameCanonical": "Echinocereus"
        }
      ]
    }
  ]
}
```