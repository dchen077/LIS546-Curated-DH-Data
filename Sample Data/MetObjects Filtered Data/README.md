# Metropolitan Museum of Art Open Access Sample Dataset

## About
The Metropolitan Museum of Art provides datasets of information on more than 470,000 artworks in its Collection for unrestricted commercial and noncommercial use. The complete data is available as CSV file on [GitHub](https://github.com/metmuseum/openaccess). The companion artworks listed in the datasets can be identified and searched in the [Collection section](https://www.metmuseum.org/art/collection) of the Museum's website. Images associated with artworks that are in the public domain are downloadable in high resolution. 

### Existing Project Data License
[CC0](https://creativecommons.org/publicdomain/zero/1.0/)

See [Open Access](https://www.metmuseum.org/policies/image-resources) page for more information on Open Access Policy.


## Data and File Information

The __MetObject_Sample_Data.csv__ is a filtered dataset that only contains objects with cultures that include the term "Chinese" or "Japanese," the period around or after the 18th century, and are in the public domain. The dataset is processed using the filtering and sorting function in Excel. 

### Sample Data Dictionary <!--this is incomplete but just to give an example of the type of data dictionary that will be included--DC-->
|Field Name|Data Type|Descripton|Example|
|---|---|---|---|
|Accession Number|Text|Unique Object Identifier|1975.433.1|
|Is Public Domain|TRUE or FALSE|Indicates whether an object's associated images are in the public domain|TRUE|
|Object Name|Text|Describes the type of object|Bust|
|Title|Text|Describes the object|Fernando VI of Spain|

_Normalization Changes that have been done to this data include:_

- Irrelevant columns including "highlighted," "Gallery Number" and "timeline work," and empty columns including "Reign," "Portfolio," "State," "Subregion," "Locale," "Locus" and "Excavation" have been deleted.

- Object Number column name is changed to Accession Number to match the metadata description of the object page in the Collection section of the Museum's website.

- Dynasty and Period columns are merged into Period. The reason for the  merge is because data about the dynasty is indicated in Period and Dynasty does not contain any data. 

The __Object Images folder__ contains digital images of four unique objects gathered from the __MetObject_Sample_Data.csv__ file and downloaded from their respective object page in the Collection Section. All images are in jpg format. 

The file names are formatted as such: 
|File Name|Accession Number.|Project Acronym|Number|
|---|---|---|---|
|Purpose|Indicate unique Object Identifier|Indicate project name|Indicate it belongs to the same ojbect|
|Example|1998.316.|DH|01|
