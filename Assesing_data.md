
### Lesson2. Lesson Outline
Data wrangling process:
> - Gather
> - Assess (this lesson)
> - Clean

Assessing your data is the second step in data wrangling. When assessing, you're like a detective at work, <br>
inspecting your dataset for two things: data quality issues (i.e. content issues) and lack of tidiness (i.e. structural issues).<br>
Assessing is the precursor to cleaning. You can't clean something that you don't know exists! <br>
In this lesson, you'll learn to identify and categorize common data quality and tidiness issues. <br>
This lesson is the shortest and most "hands-off" code-wise of all four in the course <br>
because of the passive nature of assessing relative to gathering and cleaning. <br>
We have tried to include quizzes wherever possible.<br>

This lesson will be structured as follows:
>1. You'll get motivated to assess (and later clean) the dataset for lessons 3 and 4: 
   Phase II clinical trial data that compares the efficacy and safety of a new oral insulin to treat diabetes
> 2. You'll learn to distinguish between dirty data and messy data
> 3. You'll assess the data visually and programmatically to identify:
> - Data quality issues
> - Tidiness issues
> You'll learn about data quality dimensions and categorize each of the data quality issues 
> identified above into its appropriate dimension


### Lesson5. Unclean Data: Dirty vs. Messy

There are two types of unclean data:
> - Dirty data, also known as low quality data. Low quality data has content issues.
> - Messy data, also known as untidy data. Untidy data has structural issues.

In this lesson, you are going to assess both dirty and messy data. <br>
> - Your job right now is to start to distinguish between those two now, <br>
> - even though quality and tidiness (the latter, especially) may not be 100% solidified in your mind yet.
> - Answer the following quizzes, distinguishing between low quality and untidy data, to set yourself up for success in this lesson.

> Note: the data pictured in the animation is a simplified version of the actual dataset used in this lesson.

### Lesson9. Quality: Visual Assessment1
Is it a good idea to use an integer column for storing US ZIP codes in a database?
> https://stackoverflow.com/questions/893454/is-it-a-good-idea-to-use-an-integer-column-for-storing-us-zip-codes-in-a-databas

### Lesson12. Data Quality Dimensions1
Data quality dimensions help guide your thought process while assessing and also cleaning. The four main data quality dimensions are:
- Completeness: do we have all of the records that we should? Do we have missing records or not? Are there specific rows, columns, or cells missing?
- Validity: we have the records, but they're not valid, i.e., they don't conform to a defined schema. 
  A schema is a defined set of rules for data. These rules can be real-world constraints (e.g. negative height is impossible) 
  and table-specific constraints (e.g. unique key constraints in tables).
- Accuracy: inaccurate data is wrong data that is valid. It adheres to the defined schema, but it is still incorrect. <br>
  Example: a patient's weight that is 5 lbs too heavy because the scale was faulty.
- Consistency: inconsistent data is both valid and accurate, but there are multiple correct ways of referring to the same thing. <br>
- Consistency, i.e., a standard format, in columns that represent the same data across tables and/or within tables is desired.

Regarding the other data quality research mentioned in the video, the additional dimensions are super specific cases of these four dimensions listed above. Example: currency, defined as follows: the degree to which data is current with the world that it models. Currency can measure how up-to-date data is. Currency is a specific case of accuracy data in the sense that out-of-date data is (usually) valid but wrong. In other words, our definition of accuracy can include currency.

### Lesson13. Data Quality Dimensions2
https://searchdatamanagement.techtarget.com/definition/data-quality<br>
https://www.youtube.com/watch?v=dPsx8_Fcr-U<br>
https://www.informit.com/articles/article.aspx?p=399325&seqNum=3<br>
https://www.damauk.org/RWFilePub.php?&cat=403&dx=2&ob=3&rpn=catviewleafpublic403&id=106193<br>

### Lesson14. Data Quality Dimensions1
**Assess**
> These are the programmatic assessment methods in pandas that you will probably use most often:
> * .head (DataFrame and Series)
> * .tail (DataFrame and Series)
> * .sample (DataFrame and Series)
> * .info (DataFrame only)
> * .describe (DataFrame and Series)
> * .value_counts (Series only)
> * Various methods of indexing and selecting data (.loc and bracket notation with/without boolean indexing, also .iloc)
 
### Lesson21. Assessing: Summary
Assessing is the second step in the data wrangling process:
- Gather
- Assess
- Clean

You can assess data for:
- **Quality:** <br>
  issues with content. Low quality data is also known as dirty data.
- **Tidiness:** <br>
  issues with structure that prevent easy analysis. Untidy data is also known as messy data. Tidy data requirements:
 - Each variable forms a column.
 - Each observation forms a row.
 - Each type of observational unit forms a table.

...using two types of assessment:
- **Visual assessment:**<br>
scrolling through the data in your preferred software application (Google Sheets, Excel, a text editor, etc.).
- **Programmatic assessment:**<br> 
using code to view specific portions and summaries of the data (pandas' head, tail, and info methods, for example).



