# Singapore Biographical Database 

## About

Biographical_Information.xls belongs to Singapore Biographical Database. The original [file](https://github.com/chsshgis/Singapore-Biographical-Database/blob/master/%E4%BA%BA%E7%89%A9%E6%95%B0%E6%8D%AE%201.0.xlsx) is hosted in their Github repository. The file in this repository has been normalized and standardized using OpenRefine.

## Data and File Overview

### Sample Data Dictionary <!--this is incomplete but just to give an exmaple of the type of data dictionary that will be included--DC-->
|Field Name|Data Type|Descripton|Example|
|---|---|---|---|
|NodeID| Integer|Unique ID for each biographical data point or personality.|1|
|Focused_or_Related|Text|Indicates whether the personality is a central personality (Focus) or related to a central personality (Related) | Focused |
|Chinese_Name|Text|The name of the personality in simplified Chinese|康乐公爵|
|English_Name|Text|The name of the personality in English|Lee Dai Soh|
|Pinyin_Name|Text|The name of the personality in Pinyin|Li Dasha|
|YOB|Date|The personality's year of birth|1879|
|YOB_ReferenceA|Text|The source reference for the personality's year of birth. The publication year, source title, and page numbers are included.|1896, 新华历史人物列传, p10|

***Normalization changes that have been done to this dataset include:***

- Separated Chinese and English translations into two columns.

- Standardized column names to be English only.

- Standardized null values to be Nil for columns that contain links.

- Fixed one column name translation mistake. Reference2_Complete_Index 参考文献2完整索引 was incorrectly inputted as Reference2_Short_Index.

- Minimized redundant reference titles in the index columns.

***The table below documented the eliminated column names in Chinese and the retained English column names (Extracted from original dataset)***

|Column Name English|Column Name Chinese|
|-------------------|-------------------|
| Node ID  |  人物编号 |
| Focused_or_Related | 核心人物/相关人物 |
| YOB | 出生年份 |
| YOD | 逝世年份 |
| Dialect_Group | 方言群 |
| Node_Size | 节点大小 |
| Hometown_in_Details | 细致祖籍地 |
| Search_by_Place_of_Origin | 祖籍地检索 |
| Search_by_Place_of_Birth | 出生地检索 |

Last Updated: Jun. 2, 2024 
