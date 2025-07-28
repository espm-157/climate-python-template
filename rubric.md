# Climate Module: Detailed Rubric

Total: 20 points (of 24 available -- this allows multiple paths through the module)

## 1. Data Reading and Preprocessing (**4 points**)

**4 points**: The notebook correctly reads in the data, handles missing or incorrect data appropriately, and clearly documents these steps.
 
## 2. Data Analysis and Plotting (**4 points**)

**4 points**: The data analysis is thorough, appropriate for the data, and well-executed. Plots are clear, well-labeled, and enhance understanding of the data. Figures are clearly labeled with legends, titles and axes labels.



## 3. Code Quality and Documentation (**4 points**)

**4 points**: The code should be concise, semantically meaningful. The code does not introduce additional libraries or methods not necessary for the task or beyond the scope of basic data analysis methods covered in the course so far.   

Avoid common LLM-based code-junk that does not follow best practices:
  - Do not use `print` statements in code cells.  Cells should do one clear isolated task.  The final value on a cell is auto-printed by Jupyter without needing a `print` statement -- this should be used appropriately (e.g. to display small tables or plots).  
  - Code should not include unnecessary error handling, such as `try` statements.  Use concise, working code for the data.  
  - Code should not create function definitions unless they serve a clear use in making the code more concise and readable. 
  - Do not include code comments in most cases.  Codes should be self-documenting, with clear variable names and structure.  Comments should be brief and only to clarify technical details.  Use markdown cells to explain the overall logic and flow of the notebook.
  - avoid long chunks of code that are not broken up into smaller, logical steps.  Each code cell should do one thing, and be clearly labeled with a markdown cell above it to explain what it does.

## 4. Presentation and Clarity (**4 points**)

**4 points**: The notebook is well-formatted and visually appealing, with a logical flow. Text and figures are clear, well-integrated, and free of spelling or grammatical errors.


## 5. Use of GitHub (**4 points**)

**4 points**: 

README file is updated with:
  - Authorship information
  - GitHub Actions badge, with correct link to repository
  - Updated description of repository overview.

Repository passes the auto-check on GitHub Actions.

Repository is clearly organized with logical filenames.

Clear, clean record of GitHub commits, appropriate git log messages. 
Appropriate use of branches and pull requests if indicated by the instructor.


## Failure conditions

The notebook fabricates data, or presents fictious, made-up, or "example" numbers in tables or charts as if they are real instead of reading data from the canonical data sources indicated. (Automatic fail)


