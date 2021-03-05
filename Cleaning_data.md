### Lesson3. Dataset: Oral Insulin Phase II Clinical Trial Data
https://care.diabetesjournals.org/content/38/12/2266.long
http://media.hypersites.com/clients/1446/filemanager/Articles/DocCenter_Problem_with_data.pdf

*****************************
### Lesson5. The Process
The very first thing to do before any cleaning occurs is to make a copy of each piece of data. 
All of the cleaning operations will be conducted on this copy so you can still view the original dirty and/or messy dataset later. 
Copying DataFrames in pandas is done using the copy method. 
If the original DataFrame was called df, the soon-to-be clean copy of the dataset could be named df_clean.

<details>
Nice! That's correct.
Two quality issues (wrong data type and four-digit zip codes) were cleaned at once here, 
which is perfectly okay if they are related as they were in this example.
Testing can be performed by looking at the output of patients_clean.zip_code.head(), 
inspecting the first five records of the (hopefully) clean zip code column.
</details>

https://stackoverflow.com/questions/27673231/why-should-i-make-a-copy-of-a-data-frame-in-pandas

*****************************
### Lesson8. Address Missing Data First
**Imputing** means filling in missing data values with other values, using some appropriate method. 
Here is more information on the topic of imputation: Wikipedia: Imputation
https://en.wikipedia.org/wiki/Imputation_(statistics)


*****************************
### Lesson19. The Cleaning Summary
Clean: Summary Cleaning is the third step in the data wrangling process:
- Gather
- Assess
- Clean

There are two types of cleaning:
- Manual (not recommended unless the issues are one-off occurrences)
- Programmatic

The programmatic data cleaning process:
- **Define:** convert our assessments into defined cleaning tasks. 
These definitions also serve as an instruction list so others (or yourself in the future) can look at your work and reproduce it.
- **Code:** convert those definitions to code and run that code.
- **Test:** test your dataset, visually or with code, to make sure your cleaning operations worked.

Always make copies of the original pieces of data before cleaning!

