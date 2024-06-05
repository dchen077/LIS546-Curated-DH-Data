# Data Transformation and Qualities Criteria Q&A

## Data Transfer

### How will users or curators upload data to your repository? 

Users and curators will submit their digital humanities projects via our GitHub link.This approach allows contributors to submit projects by pushing their repositories to our designated GitHub organization page, where they can be reviewed and integrated into our broader collection. Upon submission, contributors will be required to fill out a detailed survey about their project. This survey will include questions about the content, scope, relevance to modern and contemporary Chinese and Japanese studies, and any sensitive or confidential information contained within their data. 

### What kind of authenticity checks would you perform to make sure this data is what it purports to be? Does this include any virus-scanning tools?

Upon receipt of data from GitHub, several steps will be taken to verify its authenticity and ensure its safety and relevance:

__Virus Scanning__: With possible funding, we will perform a virus scan on all submitted files using robust antivirus software such as McAfee or Norton Antivirus. This is crucial to prevent the introduction of malware into our repository.

__File Integrity Checks__: We will rely on GitHub to maintain the integrity of files through version control, and ensure no 
corruption has occurred during the download process.

__Content Verification Survey__: Contributors will complete a detailed survey that includes verification of the authenticity and appropriateness of the content. This survey will ask specific questions about the sources of their data, any transformations it has undergone, and how it aligns with the project's focus on Chinese and Japanese digital humanities.

### How will you identify confidential, sensitive, or private information contained in this data? (in other words, What constitutes private or sensitive information? 

Considering the nuanced nature of digital humanities research, especially in fields involving modern historical studies of China and Japan, automated tools may not catch all sensitive content, such as culturally specific identifiers. Thus, each dataset will also undergo a manual review by team members trained in identifying sensitive information within the context of Chinese and Japanese studies.

### What is your policy for removing/redacting/protecting this kind of content?

All actions taken to manage sensitive data (redaction, restriction, encryption) will be clearly documented. This documentation will be accessible to users, providing transparency about how data has been altered from its original form and the rationale behind these changes. Furthermore, users can choose to redact and remove their deposited data without disclosing their reason. However, as mentioned earlier, the documentation of the removal of any part or the entirety of the data will be documented and openly available. 

### How will you apply an identifier to each data collection? What kind? Why?

Each data collection submitted through GitHub will be assigned a unique Digital Object Identifier (DOI). DOIs are persistent identifiers used widely across academic publications, which make digital content easily locatable and citable over the long term. 

### What additional metadata (beyond what the depositor provides) should be created at the point of data being transferred to your stewardship?

We will create additional metadata about the origin of the data, the methodology used to collect it, any changes made by the original researchers, and the context in which it was gathered. To easily locate each individual file, we will create metadata of where the file is located and which dataset collection it belongs to. 

### Is there any additional documentation that should be created in order to meaningfully preserve or use this data?

We will include documents about the storage, archiving, and preservation measures taken to ensure the long-term usability of the data. Specifically, we will include documentation on the depositor's statement on the maintenance of the dataset and scholarship and publications that have utilized or referenced the dataset. 

We recommend our depositors to provide these sections in their project READMEs, including an About section, a link to existing data licenses, information on data and files (i.e. data dictionaries), the date for when the dataset was last updated, and other sections as needed. 

## Data Transformation

File / Format

### In what formats should the data be stored? Does this differ from how it should be served to end-users? If so, how might you describe the policy for transforming data from one format to another (e.g. when you will create a CSV from a set of tables in a database)

We will store data in open, non-proprietary formats such as:

__Text Data__: Plain text (UTF-8 encoding), XML (with included or accessible schema), and PDF/A for archival purposes.

__Images__: TIFF (uncompressed) for archival quality and PNG for general use.

__Tabular Data__: CSV for its simplicity and wide support in data tools.

See our __recommend_file_format.md__ for additional information on accepted file formats. 

When data needs to be transformed from its original submission format to a preservation or user-friendly format, this will be done following clear guidelines to avoid data loss or corruption.

Transformation rules include validation of the original format, conversion using reliable tools (ensuring no loss of information), and verification post-conversion to ensure integrity.

Each transformation will be documented in the metadata, detailing the original format, the tool used for conversion, the date of conversion, and any changes in data quality or structure.

### Will you accept data that are stored in proprietary formats? How will you communicate this to users?

We will accept proprietary formats under the condition that they can be converted to open formats without significant loss of data fidelity.

### How will you record, store, and provide end-users information about what changes you’ve made to a dataset? 

Each significant change to a dataset will result in an increment of its version number, starting from 1.0 for the original submission. Also, we will make sure that metadata for each dataset will include an 'updated_last' field, which provides the date of the most recent change. This ensures users are always aware of the timeliness of the data they are accessing.
Data Values

### What steps should be taken to normalize the data? 

Here’s how we will approach the normalization process:

__Standardize Column Names__: We will implement a uniform naming convention across all datasets to avoid confusion and facilitate automated analysis. For instance, all date columns will be named in a consistent manner such as "date_published" across datasets, and all naming will adhere to a camelCase or snake_case format based on the most common usage in the existing datasets.

__Develop a Data Dictionary__: Each dataset will come with a detailed data dictionary that defines every column, the type of data it holds, and any standardized codes or abbreviations used. For example, if a dataset involves locations in Japan or China, the dictionary will detail the naming conventions used for places and any related codes.

  On __Data Dicitonary__ of a CSV file, we will make sure the depositor includes information on every field name, type of data, description of the field name, and an example. See the table below for example.
|Field Name|Type of Data|Descriptoin|Example|
|---|---|---|---|
|ID|Integer|Unique Identifier|001|

For __Data Dictionary__ of other files, the depositor will provide relevant information that describes every element of the dataset, including naming conventions and relationships between files.

__Standardize Values for Missing or Null Values__: We will standardize the representation of missing or null values across datasets using a consistent format (such as Nil or null), which will be clearly documented in the data dictionary. This ensures that users understand what a missing value represents in any dataset they work with.

__Labeling Values by Type__: Each variable in the datasets will be clearly labeled by type (e.g., text, number, boolean, categorical). This labeling will help in data type validation and ensure that data manipulation functions are appropriately applied.

__Multilingual dataset__: Given many of our datasets are in multiple languages, we aim to standardize the language of the dataset and create appropriate metadata documentation. Issues related to translation and transliteration will be carefully considered and reflected in our normalized datasets. 

### How would you help ensure that these principles are met for data that you collect?

Clear guidelines on how to format data according to tidy data principles will be provided on the repository’s website. Contributors will be encouraged to use these guidelines when preparing their data for submission. So, submissions that fail to meet tidy data standards will go through a review process where the contributor is asked to make necessary adjustments. If the contributor is unable to do so, our curatorial team will assist in reformatting the data according to tidy data principles.

## Acknowledgement

While our goal is to normalize data so it is machine and human-readable, we will also communicate with the depositor to ensure the normalization process does not sacrifice the data itself for structured order. We do not condone tidying data for the sake of tidying data. If a depositor finds the normalization process takes away the diversity of the dataset and causes the dataset to lose any value, we will respect their request and keep it as is. 

Further Reading: 

Rawson, Katie, and Trevor Muñoz. “Against Cleaning.” In Debates in the Digital Humanities 2019, edited by Matthew K. Gold and Lauren F. Klein, 279–92. University of Minnesota Press, 2019. https://doi.org/10.5749/j.ctvg251hk.26.
