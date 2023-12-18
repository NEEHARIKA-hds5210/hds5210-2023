# Feedback on your final

**Final Score: 55/60**

The grading rubric for the final can be found in GitHub: https://github.com/paulboal/hds5210-2023/blob/main/final/final-instructions.pdf

**Functional Requirements**
* 5 points - Uses data from at least two different sources: local file, internet, web service, relational database, AWS S3, etc; and formats: CSV, JSON, database, XML, Excel, etc
* 5 points - Data from multiple sources has to be joined together at least twice
* 5 points - Data is aggregated or pivoted at least twice during the program
* 5 points - Some kind of field-level transformation is performed at least 5 times
* 5 points - The program creates 3 or more data visualizations 
* 5 points - The program serves a theoretical purpose described in documentation, that could potentially do something in healthcare or another industry of interest

**Modularity / Style**
* 15 points - The code is broken up into various functions or classes to make testing and reuse easier

**Documentation and Professionalism**
* 15 points - All functions are documented and notebook cells include annotations and explanations.


**Nice opening outline.  It's a little generic, but that's OK.  The details come later.**

**(-1) From the beginning, you should tell us what is in the three datasets you're going to use.  Just telling us who provided them isn't very helpful.  All I know them as are "Dataset 1", "Dataset 2", and "Dataset 3".  I don't know how they'll be used or what they contain.**

**Note that creating a function that simply runs one line of code is usually not that helpful.  I appreciate you creating some functions and documenting them, but I'm not sure how helpful they were.**

**(-1) The variable names `xlsx`, `txt`, and `csv` are poor choices. They tell us what format the data was in, but that isn't important to our analysis.  We want to know WHAT the data is for.**

**You took the time to drop duplicates from the source files, but why? Was there any indication that there might be inappropriate duplicates.**

**(-3) When you merged `df1` and `csv` using Age, Sex, Outcome you didn't realize that your data wasn't summarized and unique at the level.  The result is that you duplicated some of your data in the join operation.  You did the same thing with `txt` and `xlsx`.  (Again, the poor variable names make it VERY hard to understand the intent here.)  Note that you can't just say "what columns are common, I'll just join on those."  The join needs to make sense with the nature of the data.**


**Overall, it was clear you put a lot of work into the final project.  I don't believe all of it was necessary, though.  If you'd been more intentional with your questions and analysis, I think you could have written a shorter final project.**